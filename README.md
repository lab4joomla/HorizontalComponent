# Horizontal component
Building middleware for a command bus to add behaviour to MVC.  Working towards a new MVC. Until now in Nooku and FOF there was much emphasis on db-behaviour, thereby staying at the db-level; I'd like to investigate to bring that to a model-level, agnostic of any persistence. The view will be a content tree, agnostic of any rendering type. See https://github.com/joomla-projects/joomla-pythagoras/blob/staging/discussion/mvc.md 

Taking tags as an example. As was done in the first try to add a tagging and versioning behaviour as a plugin by Nicholas: https://github.com/joomla-projects/joomla-pythagoras/tree/staging/plugins/behaviour . And the tagging behaviour that is now being made in Joomlatools Framework: https://github.com/joomlatools/joomlatools-todo/issues/7 

Concrete first goal: implement a tagging horizontal component as middleware for a command bus that works with Joomla's MVC.

Concrete second goal: add a component to configure all installed horizontal components for all installed vertical components. A horizontal component is by default on or off for all installed vertical components and in this ortho-configure-component we can fine-tune that for the current installation.
