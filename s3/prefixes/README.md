### Make bucket
```sh
aws s3 mb s3://prefixes-ab
```

### Create a folder object
```sh
aws s3api put-object --bucket="prefixes-ab" --key="hello/"
```

### Create many folders -> To test how many prefixes for s3 buckets : 1024 bytes
```sh
aws s3api put-object --bucket="prefixes-ab" --key="lorem/ipsum/dolor/sit/amet/consectetur/adipiscing/elit/sed/do/eiusmod/tempor/incididunt/ut/labore/et/dolore/magna/aliqua/ut/enim/ad/minim/veniam/quis/nostrud/exercitation/ullamco/laboris/nisi/ut/aliquip/ex/ea/commodo/consequat/duis/aute/irure/dolor/in/reprehenderit/in/voluptate/velit/esse/cillum/dolore/eu/fugiat/nulla/pariatur/excepteur/sint/occaecat/cupidatat/non/proident/sunt/in/culpa/qui/officia/deserunt/mollit/anim/id/est/laborum/sed/ut/perspiciatis/unde/omnis/iste/natus/error/sit/voluptatem/accusantium/doloremque/laudantium/totam/eaque/ipsa/quae/ab/illo/inventore/veritatis/et/quasi/architecto/beatae/vitae/dicta/sunt/explicabo/nemo/enim/ipsam/voluptatem/quia/voluptas/sit/aspernatur/aut/odit/aut/fugit/sed/quia/consequuntur/magni/dolores/eos/qui/ratione/voluptatem/sequi/nesciunt/porro/quisquam/est/qui/dolorem/ipsum/quia/dolor/sit/amet/consectetur/adipisci/velit/sed/quia/non/numquam/eius/modi/tempora/incidunt/ut/labore/et/dolore/magna/aliquam/quaerat/voluptatem/ut/enim/ad/minima/veniam/quis/nostrum/exercitationem/ullam/corporis/suscipit/laboriosam/nisl/ut/aliquid/ex/ea/commodo/consequatur/aut/necessitatibus/sed/repudiandae/itaque/earum/rerum/hic/tenetur/a/sapiente/delectus/ut/aut/"
```
