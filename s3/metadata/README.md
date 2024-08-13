### Upload a file with a user defined metadata
```sh
aws s3api put-object --bucket prefixes-ab --key="hello/hello.txt" --metadata Planet=Mars
```

### Get Metadata through head object
```sh
aws s3api head-object --bucket prefixes-ab --key="hello/hello.txt"
```