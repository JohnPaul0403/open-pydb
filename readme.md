# Open-PyDB

An unstructured database module for Python

Open-PyDB is a simple, lightweight, and flexible open-source database for that allows users to make use of unstruct data. It provides a simple, flexible and extensible way to data. The project contains the code for a simple database manager using a Client class to interact with a database The database manager supports creating and deleting databases and collections, as well as adding and deleting data from collections.

---

## Instalation

### For Windows

```Python
pip install open-pydb
```

### For Mac and Linux

```Python
pip3 install open-pydb
```

## Usage

Here's an example of how to use Open-DB:

```Python
from open_pydb import Client

# Create a new client
client = Client()

# Add a new database
db = client.add_db("Users")

# Get the database
db = client.get_db()

# Get the collections in the database
collections = db.get_collections()

# Add data to the first collection
collections[0].add_data(id="2", name="Get with me")

# Delete data from the first collection
collections[0].delete_data(collections[0].data)
```

## Data Model

Open-DB uses a simple data model based on the Data class. Here's an example of how to use the Data class:

```Python
from open_pydb import Data

# Create a new data object
data = Data(foo='bar', baz=42)

# Convert the data object to a JSON string
json_data = data.to_json()

# Convert a JSON string to a data object
new_data = Data.from_json(json_data)
```

## Contributing

We welcome contributions to Open-DB! If you'd like to contribute, please fork the repository and make your changes in a new branch. Once you're ready to submit your changes, open a pull request and we'll review your changes as soon as possible.

## License

Open-DB is released under the MIT License. See the LICENSE file for details.

## Contact

For any questions or issues, please feel free to contact at [johnpar2004@gaml.com](johnpar2004@gmail.com).
