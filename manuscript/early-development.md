# {{ book.sections.overview.early-development }}

Authoring a project in any modern CMS begins with the tools chosen to author it *with*.

Drupal is fully featured and capable of huge layers of **extensibility**. Extensibilty, meaning 'able to be made bigger' (basically). This is a small piece of a concept that will be defined later in the book called **modularity**. Modularity can be thought of by imaginging a computer with a single *virtual* motherboard. Because the foundation of the computer is virtual, it can be upgraded piece-by-piece, part-by-part until the new system has no relation to the old, yet is infinitely better.

## Modularity

Both the Open Source Community and Drupal thrive on the concept of Modularity (and the Design Systems fuelling it).

A good comparison to make would be setting aside the parts and tools needed to build a house.

Because the Open Source Community continually improves on everything within itself, no version of Drupal will ever come with all the tools a Web Author will need to succeed. It will always come with the tools needed to succeed, have no doubt of that, but not the **best** tools.

### Here are a few examples of tools that can make a new Web Author's life a little easier in Drupal:
#### That are mostly used only for Drupal
* [Kalabox](http://www.kalabox.io/ "Kalabox") - Push-click installation of local Backdrop, Drupal 7, Drupal 8, and/or Wordpress installations. A fairly slick tool for scaffolding, building, and creating web systems without the massive complexity involved with the typical Development Process that has existed until recent years.
* [Jeff Geerling's](http://jeffgeerling.com/ "Jeff Geerling's Website") [Drupal VM](http://www.drupalvm.com "Drupal VM"),
* [Moshe Weitzman's](https://www.drupal.org/u/moshe-weitzman "Moshe Weitzman's Website") [Drush](https://github.com/drush-ops/drush "Drush"),
* [Dmytro Danylevskyi's](http://dmytro.danylevskyi.com/ "Dmytro Danylevskyi's Website") [Vagrant Drupal Development](http://www.drupalvm.com "Vagrant Drupal Development") platform,
* [Acquia's](https://www.acquia.com/ "Acquia's Website") [Acquia Dev Desktop](https://www.acquia.com/downloads "Acquia Dev Desktop"),
* [Phase 2's](https://www.phase2technology.com "Phase 2's Website") [DevTools.io](http://phase2.github.io/devtools/ "DevTools.io"),
* [Four Kitchens'](http://fourkitchens.com/ "Four Kitchens") [Aquifer.io](http://aquifer.io/ "DevTools CLI"),
* [Pantheon.io](https://pantheon.io/ "Pantheon.io'"),
* [Pantheon.io's](https://pantheon.io/ "Pantheon.io'") [Terminus CLI](https://pantheon.io/docs/terminus/ "Terminus CLI"),
* [Drupal Console](https://drupalconsole.com/ "Drupal Console"),
 * and many others...

## Modern Drupal Web Authoring

For the workflow in *this* book, we will be using only the following tools, with careful work instructions (so don't get overwhelmed!).

* [Kalabox](http://www.kalabox.io/ "Kalabox") *(or Geerling's Drupal VM)*
* [Jeff Geerling's](http://jeffgeerling.com/ "Jeff Geerling's Website") [Drupal VM](http://www.drupalvm.com "Drupal VM"),
* [Moshe Weitzman's](https://www.drupal.org/u/moshe-weitzman "Moshe Weitzman's Website") [Drush](https://github.com/drush-ops/drush "Drush"),
* [Pantheon.io](https://pantheon.io/ "Pantheon.io'"),
* [GitHub](https://github.com/ "GitHub"),
* a text editor of your choice, and,
* an IDE of your choice.

In the next few sections, we will walk slowly through creating an account and logging in with GitHub, Pantheon, and Drupal.org, followed by downloading and installing either Kalabox or Drupal VM for local development.

Kalabox allows for a faster and more efficient development time, but Drupal VM is infinitely more extensible (modular), though only when using Ansible on either Mac OSX or Linux boxes. We will be using Kalabox within this book primarily however because it is fully cross-compatible on **all** systems, Windows included.

