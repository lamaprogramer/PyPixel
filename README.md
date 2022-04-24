# PyPixel
Simple Python library allowing you to use the Hypixel API from your terminal


# Installation and Importing
To install the PyPixel library, use:

```
pip install MCPyPixelAPI
```

Then to import it you can use:

```python
import PyPixel
# OR
from PyPixel import Hypixel
```

# Usage
In order to to use the PyPixel library, you first need your "Hypixel API Key".

To get your API key you need to:

### 1). Log onto the Hypixel Minecraft server

### 2). Run the `/key` command (This should output a string of random letters, numbers and charactors)

### 3). Copy the output, and paste it as the first parameter of the Hypixel class:

```python
Hypixel("YOUR API KEY")
```

Now you need the UUID of your Minecraft player, to do this:

### 1). Go to [NameMC](https://namemc.com)

### 2). Type in your username in the search bar

## 3). Click on your profile and copy the UUID

Now you can paste your player uuid as the second parameter of the Hypixel Class, it should now look like:

```python
Hypixel("YOUR API KEY", "YOUR UUID")
```
Now you are all set to start using the Library!

# Documentation

The documentation for all of the existing library Classes, Methods, and parameters

## Classes

### Hypixel()
**parameters:** api_key, uuid
**desc:** Body of the library
```python
Hypixel(api_key, uuid)
```
## Methods

### rawdata()
**parameters:** (username: string)

**desc:** returns all of the selected player's data as a `dictionary`
```python
Hypixel(api_key, uuid).rawdata(username)
# OR
hp = Hypixel(api_key, uuid)
hp.rawdata(username)
```

### getkey()
**parameters:** (*optional* isVerbose: Bool)

**desc:** returns player's API key(if they have one)
```python
Hypixel(api_key, uuid).getkey()
# OR
hp = Hypixel(api_key, uuid)
hp.getkey()
```

### achievements()
**parameters:** (username: string)

**desc:** shows all of selected player's achievement data
```python
Hypixel(api_key, uuid).achievements(username)
# OR
hp = Hypixel(api_key, uuid)
hp.achievements(username)
```

### recentgames()
**parameters:** (username: string)

**desc:** shows all of selected player's recent games
```python
Hypixel(api_key, uuid).recentgames(username)
# OR
hp = Hypixel(api_key, uuid)
hp.recentgames(username)
```

### friends()
**parameters:** (username: string)

**desc:** shows selected player's friends list and online status
```python
Hypixel(api_key, uuid).friends(username)
# OR
hp = Hypixel(api_key, uuid)
hp.friends(username)
```

### status()
**parameters:** (username: string)

**desc:** shows selected player's online status
```python
Hypixel(api_key, uuid).status(username)
# OR
hp = Hypixel(api_key, uuid)
hp.status(username)
```
