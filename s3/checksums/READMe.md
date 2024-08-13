### S3 Checksums
--- s3 use checksums to validate the integrity of files/objects in transit

### Create a new s3 bucket

```md
aws s3 mb s3://checksums-example
```

## Create a file that we will do a checksum on it

```sh
sudo apt install rhash -y
rhash --crc32 myfile.txt
```

```sh
aws s3api put-object \
--bucket checksums-example \
--key myfilecrc32.txt \
--body myfile.txt \
--checksum-algorithm="CRC32" \
--checksum-crc32="E7C80B87"
```

```
echo "Hello Mars" > myfile.txt
```

## Get a checksum of a file for md5
```
md5sum myfile.txt
```

```
aws s3 cp myfile.txt s3://checksums-example
aws s3api head-object --bucket checksums-example --key myfile.txt
```
