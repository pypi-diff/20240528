# Comparing `tmp/daalab-1.3.tar.gz` & `tmp/daalab-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daalab-1.3.tar", last modified: Tue May 28 03:04:00 2024, max compression
+gzip compressed data, was "daalab-1.4.tar", last modified: Tue May 28 04:30:35 2024, max compression
```

## Comparing `daalab-1.3.tar` & `daalab-1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 03:04:00.199565 daalab-1.3/
--rw-rw-rw-   0        0        0      153 2024-05-28 03:04:00.198567 daalab-1.3/PKG-INFO
--rw-rw-rw-   0        0        0      568 2024-05-27 15:44:09.000000 daalab-1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 03:04:00.167212 daalab-1.3/daalab/
--rw-rw-rw-   0        0        0     1084 2024-05-28 03:03:05.000000 daalab-1.3/daalab/__init__.py
--rw-rw-rw-   0        0        0    41996 2024-05-28 03:02:19.000000 daalab-1.3/daalab/codes.py
--rw-rw-rw-   0        0        0     1363 2024-05-27 15:44:10.000000 daalab-1.3/daalab/testing.py
-drwxrwxrwx   0        0        0        0 2024-05-28 03:04:00.194571 daalab-1.3/daalab.egg-info/
--rw-rw-rw-   0        0        0      153 2024-05-28 03:04:00.000000 daalab-1.3/daalab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2024-05-28 03:04:00.000000 daalab-1.3/daalab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 03:04:00.000000 daalab-1.3/daalab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-28 03:04:00.000000 daalab-1.3/daalab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 03:04:00.200565 daalab-1.3/setup.cfg
--rw-rw-rw-   0        0        0      269 2024-05-28 03:03:13.000000 daalab-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 04:30:35.513653 daalab-1.4/
+-rw-rw-rw-   0        0        0      153 2024-05-28 04:30:35.511650 daalab-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2024-05-27 15:44:09.000000 daalab-1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 04:30:35.492653 daalab-1.4/daalab/
+-rw-rw-rw-   0        0        0     1464 2024-05-28 03:30:13.000000 daalab-1.4/daalab/__init__.py
+-rw-rw-rw-   0        0        0    47341 2024-05-28 03:30:16.000000 daalab-1.4/daalab/codes.py
+-rw-rw-rw-   0        0        0     1363 2024-05-27 15:44:10.000000 daalab-1.4/daalab/testing.py
+drwxrwxrwx   0        0        0        0 2024-05-28 04:30:35.509650 daalab-1.4/daalab.egg-info/
+-rw-rw-rw-   0        0        0      153 2024-05-28 04:30:35.000000 daalab-1.4/daalab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2024-05-28 04:30:35.000000 daalab-1.4/daalab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 04:30:35.000000 daalab-1.4/daalab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-28 04:30:35.000000 daalab-1.4/daalab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 04:30:35.513653 daalab-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      269 2024-05-28 04:30:30.000000 daalab-1.4/setup.py
```

### Comparing `daalab-1.3/README.md` & `daalab-1.4/README.md`

 * *Files identical despite different names*

### Comparing `daalab-1.3/daalab/codes.py` & `daalab-1.4/daalab/codes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1602,7 +1602,203 @@
             </Routes>
           </div>
         </Router>
       );
     }
     export default App;'''
     print(code)
+
+def print_routingserver():
+    code = '''// server.js
+
+    const http = require('http');
+    const fs = require('fs');
+    const path = require('path');
+
+    const server = http.createServer((req, res) => {
+      if (req.url === '/page1') {
+        fs.readFile(path.join(__dirname, 'page1.html'), (err, data) => {
+          res.writeHead(200, {'Content-Type': 'text/html'});
+          res.end(data);
+        });
+      } else if (req.url === '/page2') {
+        fs.readFile(path.join(__dirname, 'page2.html'), (err, data) => {
+          res.writeHead(200, {'Content-Type': 'text/html'});
+          res.end(data);
+        });
+      } else {
+        fs.readFile(path.join(__dirname, 'index.html'), (err, data) => {
+          res.writeHead(200, {'Content-Type': 'text/html'});
+          res.end(data);
+        });
+      }
+    });
+
+    const PORT = process.env.PORT || 3000;
+    server.listen(PORT, () => {
+      console.log(`.`);
+    });
+    '''
+    print(code)
+
+def print_es5vses6():
+    code='''//es5.js
+    function factorialES5(num) {
+      if (num === 0 || num === 1) {
+        return 1;
+      }
+      var result = 1;
+      for (var i = num; i >= 1; i--) {
+        result *= i;
+      }
+      return result;
+    }
+    console.log(factorialES5(5));
+    //es6.js
+    const factorialES6 = (num) => {
+      if (num === 0 || num === 1) {
+        return 1;
+      }
+      let result = 1;
+      for (let i = num; i >= 1; i--) {
+        result *= i;
+      }
+      return result;
+    }
+    console.log(factorialES6(5));
+
+    '''
+    print(code)
+
+def print_funclass():
+    code='''create a react app , in src create this file -->
+    fruitsFunctional.jsx
+    import React from 'react';
+
+    const FruitTableRow = ({ name, color, price }) => {
+      return (
+        <tr>
+          <td>{name}</td>
+          <td>{color}</td>
+          <td>{price}</td>
+        </tr>
+      );
+    };
+
+    export default FruitTableRow;
+
+    in src create --> fruitsClass.jsx
+    import React, { Component } from 'react';
+    import FruitTableRow from './fruitsFunctional';
+    import './fruitsClass.css'
+
+    class FruitTable extends Component {
+      constructor(props) {
+        super(props);
+        this.state = {
+          fruits: [
+            { name: 'Apple', color: 'Red', price: '20rs' },
+            { name: 'Banana', color: 'Yellow', price: '5rs' },
+            { name: 'Orange', color: 'Orange', price: '15rs' },
+          ],
+        };
+      }
+
+      render() {
+        return (
+          <div>
+            <h1>This table has been created using Functional and CLass Components...</h1>
+            <div className='centerr'>
+                <h2>Fruits Table</h2>
+                <div className='colorr'>
+                    <table>
+                      <thead>
+                        <tr>
+                          <th>Name</th>
+                          <th>Color</th>
+                          <th>Price</th>
+                        </tr>
+                      </thead>
+                      <tbody>
+                        {this.state.fruits.map((fruit, index) => (
+                          <FruitTableRow
+                            key={index}
+                            name={fruit.name}
+                            color={fruit.color}
+                            price={fruit.price}
+                          />
+                        ))}
+                      </tbody>
+                    </table>
+                </div>
+
+            </div>
+          </div>
+        );
+      }
+    }
+
+    export default FruitTable;
+
+    in src --> fruitsClass.css
+    .centerr {
+        display: flex;
+        justify-content: center;
+        align-items: center;
+        flex-direction: column;
+    }
+
+    .colorr {
+        background-color: beige;
+    }
+
+    table, th , td {
+        border: 2px solid black;
+    }
+
+    th ,td {
+        padding: 10px 30px;
+    }
+
+
+    App.js -->
+
+    import './App.css';
+    import FruitTable from './fruitsClass';
+
+    function App() {
+      return (
+        <FruitTable />
+      );
+    }
+
+    export default App;'''
+    print(code)
+
+def print_mongo():
+    code = '''npm install mongod
+    install mongo community edition from site
+    add C:\Program Files\MongoDB\Server\7.0\bin to path
+    terminal --> mongod
+    node mongoo.js
+    //code: 
+    const MongoClient = require('mongodb').MongoClient;
+    const url = 'mongodb://localhost:27017';
+    const dbName = 'mydatabase';
+    const client = new MongoClient(url);
+    async function main() {
+        await client.connect();
+        console.log('Connected to the MongoDB server');
+        const db = client.db(dbName);
+        const collection = db.collection('documents');
+        const document = { name: 'John', age: 30 };
+        const result = await collection.insertOne(document);
+        console.log('Inserted document with id: ', result.insertedId);
+        const foundDocument = await collection.findOne({ name: 'John' });
+        console.log('Found document: ', foundDocument);
+        const updateResult = await collection.updateOne({ name: 'John' }, { $set: { age: 31 } });
+        console.log('Updated document count: ', updateResult.modifiedCount);
+        const deleteResult = await collection.deleteOne({ name: 'John' });
+        console.log('Deleted document count: ', deleteResult.deletedCount);
+        await client.close(); }
+    main();'''
+    print(code)
```

### Comparing `daalab-1.3/daalab/testing.py` & `daalab-1.4/daalab/testing.py`

 * *Files identical despite different names*

