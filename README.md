# alu-AirBnB

A simplified clone of the AirBnB platform.

---

## 🌐 Project Overview

This project is a basic clone of the AirBnB web application. It features:

- A command-line interface (CLI) for managing data
- Back-end logic with data persistence
- A foundation for future front-end and API integration

Currently, it focuses on building core classes and a console for basic operations such as creating, viewing, updating, and deleting objects.

---

## 🛠️ Getting Started

### 1. Clone the Repository

Use Git to clone this project to your local machine:

```bash
git clone https://github.com/yourusername/AirBnB_clone.git
```

### 2. Run the Console

Navigate into the project folder and start the console:

```bash
cd AirBnB_clone
./console.py
```

You should now see the prompt:

```bash
(hbnb)
```

---

## 💻 Available Commands

Here are the main commands you can use inside the (hbnb) console:

| Command        | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| create         | Creates a new object instance                                               |
| show           | Displays an object by class name and ID                                    |
| destroy        | Deletes an object by class name and ID                                     |
| all            | Lists all objects (or all objects of a given class)                        |
| update         | Updates attributes of an object using class name and ID                    |
| quit / EOF     | Exits the console                                                           |

---

## 🧠 Advanced Syntax

You can also use an object-oriented style for commands:

```bash
<ClassName>.command(arguments)
```

Examples:

- `User.all()` — Lists all User objects
- `User.show("id")` — Displays a User by ID
- `User.destroy("id")` — Deletes a User by ID
- `User.update("id", "attribute", "value")` — Updates one attribute
- `User.update("id", {"attr1": "val1", "attr2": "val2"})` — Updates multiple attributes at once

---

## 🔍 Examples

### Create an object

```bash
(hbnb) create BaseModel
# Returns an ID like: 3aa5babc-efb6-4041-bfe9-3cc9727588f8
```

### Show an object

```bash
(hbnb) show BaseModel 3aa5babc-efb6-4041-bfe9-3cc9727588f8
```

### Destroy an object

```bash
(hbnb) destroy BaseModel 3aa5babc-efb6-4041-bfe9-3cc9727588f8
```

### Update an object

```bash
(hbnb) update BaseModel <id> first_name "John"
```

Or using advanced syntax:

```bash
(hbnb) BaseModel.update("<id>", {"first_name": "Jane", "age": 30})
```

---

This project is a foundation for a full-featured web application. As development continues, it will grow to include database integration, RESTful APIs, and a front-end interface.
