======================
Mail Recipient Uncheck
======================

.. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Mature-brightgreen.png
    :target: https://odoo-community.org/page/development-status
    :alt: Mature
.. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
    :alt: License: AGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fsocial-lightgray.png?logo=github
    :target: https://github.com/OCA/social/tree/12.0/mail_recipient_uncheck
    :alt: OCA/social
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/social-12-0/social-12-0-mail_recipient_uncheck
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runbot-Try%20me-875A7B.png
    :target: https://runbot.odoo-community.org/runbot/205/12.0
    :alt: Try me on Runbot

|badge1| |badge2| |badge3| |badge4| |badge5| 

When you click on *Send a message* in the Open Chatter,
Odoo displays the Message Composer:

|composer|

.. |composer| image:: composer.png
   :alt: Message Composer

You may notice that it adds suggestions of recipients:
here *Ready Mat (ready.mat28@example.com)*

These suggestions can be useful, but having them checked by default
is dangerous: for example a user could mistakenly send
a sensitive internal message to a customer.

The purpose of this module is to make sure that these suggestions
are not checked by default.

**Table of contents**

.. contents::
   :local:

Development
===========

The list of suggested partners is retrieved by a rpc call
to ``model:message_get_suggested_recipients()``

See here_ for its default implementation.

.. _here: https://github.com/odoo/odoo/blob/324634da3debefd834b4b5dcf8509da25348324d/addons/mail/models/mail_thread.py#L1740

Changelog
=========

This module is a follow-up to the old ``web_recipients_uncheck``,
available for 7.0_ and 8.0_

.. _7.0: https://github.com/OCA/web/tree/7.0/web_recipients_uncheck
.. _8.0: https://github.com/OCA/web/tree/8.0/web_recipients_uncheck

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/social/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us smashing it by providing a detailed and welcomed
`feedback <https://github.com/OCA/social/issues/new?body=module:%20mail_recipient_uncheck%0Aversion:%2012.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
~~~~~~~

* Trobz

Contributors
~~~~~~~~~~~~

 * Nils Hamerlinck <nils@trobz.com>

Maintainers
~~~~~~~~~~~

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

.. |maintainer-nilshamerlinck| image:: https://github.com/nilshamerlinck.png?size=40px
    :target: https://github.com/nilshamerlinck
    :alt: nilshamerlinck

Current `maintainer <https://odoo-community.org/page/maintainer-role>`__:

|maintainer-nilshamerlinck| 

This module is part of the `OCA/social <https://github.com/OCA/social/tree/12.0/mail_recipient_uncheck>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
