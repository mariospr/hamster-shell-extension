Hamster Gnome Shell extension
===============================

A Simple Hamster shell extension for Gnome 3.

News
-----
Frederic Guilbault (@border0464111) agreed to step up to the challenge and will
take over responsibility of the *Hamster-Shell-Extension* as new maintainer.
Thank you Frederic!

Install
--------

Dependencies
~~~~~~~~~~~~
Because *Hamster-Shell-Extension* is just a frontend to the hamster dbus
service the presence of `hamster-time-tracker
<https://github.com/projecthamster/hamster>`_ is required. You can verify that
the relevant dbus services are up and running by issuing ``ps aux | grep
hamster`` which should bring up ``hamster-service`` and
``hamster-windows-service``.

Install For Production
~~~~~~~~~~~~~~~~~~~~~~~
The extension is available on `the central extension repository <https://extensions.gnome.org/extension/425/project-hamster-extension>`_.

Current compatible Gnome shell version: 3.20
For previous shell versions check `releases <https://github.com/projecthamster/shell-extension/tags>`_.

Manual Installation For Testing and Development
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Clone the repository::

    git clone git@github.com:projecthamster/hamster-shell-extension.git

Make sure you are on the development branch::

    git checkout develop

Build a fresh distribution package::

    make dist

Extract the resulting tarball within the ``dist`` dir under the following directory::

    ~/.local/share/gnome-shell/extensions/``

After that you can enable the extension and change the preferences using Tweak
Tool, or on ``https://extensions.gnome.org/local/``
