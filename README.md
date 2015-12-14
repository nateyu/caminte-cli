## CaminteJS CLI

  Command line interface for CaminteJS ORM

## Installation

    $ npm install -g caminte-cli
    
### Options

    -h, --help                  output usage information
    -V, --version               output the version number
    -i, --iinit                 create caminte sctructure
    -g, --model <modelname>     generate data model
    -a, --adapter               database adapter (mysql|redis|etc...)
    -f, --force                 force on non-empty directory

## Quick Start

 The quickest way to get started with caminte is to utilize the executable `caminte(1)` to create an application as shown below:

Create structure:

    $ caminte -i
    
Create model:

    $ caminte -m User active:int name email password note:text created:date
    
Create routes:

    $ caminte -r user
    
Create model and routes:

    $ caminte -c Post published:bool title content:text created:date


### CaminteJS ORM db adapters:
    mysql, sqlite3, postgres, mongodb, redis, riak, couchdb(nano), rethinkdb, tingodb

<table>
    <tr>
      <td><img width="100" src="https://github.com/biggora/caminte/raw/master/media/memory.png"/></td>
      <td><img width="100" src="https://github.com/biggora/caminte/raw/master/media/mongodb.png"/></td>
      <td><img width="100" src="https://github.com/biggora/caminte/raw/master/media/mysql.png"/></td>
      <td><img width="100" src="https://github.com/biggora/caminte/raw/master/media/postgresql.png"/></td>
      <td><img width="100" src="https://github.com/biggora/caminte/raw/master/media/sqlite.png"/></td>
      <td><img width="100" src="https://github.com/biggora/caminte/raw/master/media/mariadb.png"/></td>
      <td><img width="100" src="https://github.com/biggora/caminte/raw/master/media/firebird.png"/></td>   
    </tr>
    <tr>
      <td><img width="100" src="https://github.com/biggora/caminte/raw/master/media/couchdb.png"/></td>
      <td><img width="100" src="https://github.com/biggora/caminte/raw/master/media/rethinkdb.png"/></td>
      <td><img width="100" src="https://github.com/biggora/caminte/raw/master/media/redis.png"/></td> 
      <td><img width="100" src="https://github.com/biggora/caminte/raw/master/media/tingodb.png"/></td>      
      <td><img width="100" src="https://github.com/biggora/caminte/raw/master/media/neo4j.png"/></td> 
      <td><img width="100" src="https://github.com/biggora/caminte/raw/master/media/arangodb.png"/></td>
      <td><img width="100" src="https://github.com/biggora/caminte/raw/master/media/cassandra.png"/></td>
    </tr>
</table>


### Routes

will provide the following routes:

    method        route                    action 
    ------------------------------------------------------------
    GET           /:table                  index      
    GET           /:table/:id              show       
    POST          /:table                  create    
    PUT           /:table/:id              update      
    DELETE        /:table/:id              destroy 

### Directory structure

On initialization directories tree generated, like that:

    .
    | 
    |-- models
    |   |-- User.js
    |   `-- ...
    |-- routes
    |   `-- users.js
    |       `-- ...
    `-- database.js


### Recommend extensions

- [TrinteJS](http://www.trintejs.com/) - Javascrpt MVC Framework for Node.JS
- [CaminteJS](http://www.camintejs.com/) - Cross-db ORM for NodeJS
- [2CO](https://github.com/biggora/2co) - is the module that will provide nodejs adapters for 2checkout API payment gateway.

## License

(The MIT License)
 
Copyright (c) 2014 Aleksej Gordejev &lt;aleksej@gordejev.lv&gt;

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Resources

- Visit the [author website](http://www.gordejev.lv).
- Follow [@biggora](https://twitter.com/#!/biggora) on Twitter for updates.
- Report issues on the [github issues](https://github.com/biggora/caminte-cli/issues) page.

[![Analytics](https://ga-beacon.appspot.com/UA-22788134-5/caminte-cli/readme)](https://github.com/igrigorik/ga-beacon) [![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/biggora/caminte-cli/trend.png)](https://bitdeli.com/free "Bitdeli Badge")