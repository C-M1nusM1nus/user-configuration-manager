# User Configuration Manager
A simple Python program for managing user settings. It allows you to add, update, delete, and view settings stored in a dictionary.

# Features
* **Add a setting** — Adds a new setting if the key does not already exist.
* **Update a setting** — Changes the value of an existing setting.
* **Delete a setting** — Removes an existing setting.
* **View settings** — Displays all currently stored settings.
* **Case-insensitive values** — Setting keys and values are converted to lowercase.

# Example Settings
The program includes the following test settings:

test_settings = {
    "theme": "dark",
    "language": "english",
    "notifications": "enabled"
}

# Functions
## add_setting(settings, setting)
Adds a new setting to the dictionary.

add_setting(settings, ("font", "Arial"))

If the setting already exists, an error message is returned instead.

## update_setting(settings, setting)
Updates the value of an existing setting.

update_setting(settings, ("theme", "light"))

If the setting does not exist, the function returns an error message.

## delete_setting(settings, key)
Deletes a setting from the dictionary.

delete_setting(settings, "theme")

If the setting cannot be found, "Setting not found!" is returned.

## view_settings(settings)
Displays all settings currently stored in the dictionary.

Example output:

Current User Settings:
Theme: dark
Language: english
Notifications: enabled

# Requirements
* Python 3.x
* No external libraries are required.
