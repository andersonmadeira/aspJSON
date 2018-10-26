# aspJSON

### 1. Before you jump in...

Version 1.17 of this library was originally developed by Gerrit van Kuipers. 
Since I was unable to contact him or find a public repository hosting this code, I decided to publish this library so other people could benefit of it as I did, 
and maybe we can improve it a little bit.

### 2. How to use it

To create a new json object:

```asp
Set jsonObj = New aspJSON
```

#### 2.1. Loading from source:

From string:

```asp
jsonObj.loadJSON(json_string)
```

From a .json file:

```asp
jsonObj.loadFromFile("sample.json")
```

#### 2.2 Manipulating:

Getting value of item:

```asp
jsonObj.data("key")
```

Getting value of sub item:

```asp
jsonObj.data("key").item("child")
```

Changing data:

```asp
jsonObj.data("key") = "value"
```

Converting to string:

```asp
json_object.JSONoutput()
```

#### 2.3. Creating a json object from scratch:

```asp
Set json_object = New aspJSON

json_object.data.Add "user", user 
json_object.data.Add "pass", pass
```

### 3. Contributions

Are always welcome.
