# Each module consists of a page, its respective GetXController and its dependencies or Bindings.
# We treat each screen as an independent module, as it has its only controller, and can also contain its dependencies.
# If you use reusable widgets in this, and only in this module, you can choose to add a folder for them.
   
# The Binding class is a class that decouples dependency injection, while "binding" routes to the state manager and the dependency manager.
# This lets you know which screen is being displayed when a specific controller is used and knows where and how to dispose of it.
# In addition, the Binding class allows you to have SmartManager configuration control.
# You can configure how dependencies are to be organized and remove a route from the stack, or when the widget used for disposition, or none of them.
# The decision to transfer the repositories "globally" to internal modes within each module is that we can use a function in different modules, but the problem was due to having to import more than one repository in the controller, so we can repeat the same calls functions, internal repositories, thus maintaining faster maintenance, making everything that gives life to the module reachable through the module itself.
# Repositories then become just a class to point to the controllers of our module, which and which provider we are going to consume, the same goes for services, services that have integration with some provider, must have its own repository
