.. include:: images.rst

.. _staff-client-label:

Staff client
------------------------------

*Get there:* More > Administration > Global system preferences > Staff
client

.. _staffappearance-label:

Appearance
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. _display856uasimage-label:

Display856uAsImage
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: Neither details or results page

Asks: Display the URI in the 856u field as an image on: \_\_\_

Values:

-  Both results and details pages

   -  **Important**

          Both :ref:`XSLTDetailsDisplay` and
          :ref:`XSLTResultsDisplay` need to
          have values in order for this preference to work.

   -  **Important**

          This is only implemented for MARC21.

-  Detail page only

   -  **Important**

          :ref:`XSLTDetailsDisplay` needs to
          have a value in it for this preference to work.

   -  **Important**

          This is only implemented for MARC21 and UNIMARC.

   |image113|

-  Neither details or results page

-  Results page only

   -  **Important**

          :ref:`XSLTResultsDisplay` needs to
          have a value in it for this preference to work.

   -  **Important**

          This is only implemented for MARC21 and NORMARC.

Description:

-  In addition to this option being set, the corresponding XSLT option
   must be turned on. Also, the corresponding 856q field must have a
   valid MIME image extension (e.g., "jpg") or MIME image type (i.e.
   starting with "image/"), or the generic indicator "img" entered in
   the field. When all of the requirements are met, an image file will
   be displayed instead of the standard link text. Clicking on the image
   will open it in the same way as clicking on the link text. When you
   click on the image it should open to full size, in the current window.

   |image114|

.. _displayiconsxslt-label:

DisplayIconsXSLT
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: \_\_\_ the format, audience, and material type icons and descriptions in 
XSLT MARC21 results and detail pages in the staff client.

Default: Show

Values:

-  Don't show

-  Show

   |image115|

    **Note**

    See the :ref:`XSLT material type icons <material-type-cataloging-guide-label>`
    for more information on these icons.

    **Important**

    This is only used in XSLT displays, so :ref:`XSLTResultsDisplay` and/or 
    :ref:`XSLTDetailsDisplay` must be set to use an XSLT stylesheet for 
    this to show (default or custom)

.. _intranet-includes-label:

intranet\_includes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: includes

Asks: Use include files from the \_\_\_ directory in the template
directory, instead of includes/. (Leave blank to disable)

.. _intranetcirculationhomehtml-label:

IntranetCirculationHomeHTML
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Show the following HTML in its own div on the bottom of the home
page of the circulation module:

    |image1198|

.. _intranetcolorstylesheet-label:

intranetcolorstylesheet
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Include the additional CSS stylesheet \_\_\_ to override specified
settings from the default stylesheet

Description:

-  This preference is used to set the background color and style of the
   staff client. The value is a .css file. The system administrator
   should determine which file is appropriate. Enter just a filename, a
   full local path or a complete URL starting with http:// (if the file
   lives on a remote server). Please note that if you just enter a
   filename, the file should be in the css subdirectory for each active
   theme and language within the Koha templates directory. A full local
   path is expected to start from your HTTP document root.

    **Important**

    Leave this field blank to disable.

.. _intranetfavicon-label:

IntranetFavicon
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Use the image at \_\_\_ for the staff client's favicon.

    **Important**

    This should be a complete URL, starting with http://

    **Note**

    Turn your logo into a favicon with the `Favicon
    Generator <http://antifavicon.com/>`__.

Description:

-  The favicon is the little icon that appears next to the URL in the
   address bar in most browsers. The default value for this field (if
   left blank) is the small 'K' in the Koha logo.

   |image116|

.. _intranetmainuserblock-label:

IntranetmainUserblock
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Show the following HTML in its own column on the main page of the
staff client

|image117|

|image118|

.. _intranetnav-label:

IntranetNav
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Show the following HTML in the More menu at the top of each page
on the staff client (should be a list of links or blank)

.. _intranetreportshomehtml-label:

IntranetReportsHomeHTML
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Show the following HTML in its own div on the bottom of the home
page of the reports module:

    |image1199|

.. _intranetslipprinterjs-label:

IntranetSlipPrinterJS
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Use the following JavaScript for printing slips.

Description:

-  The most logical use of this preference is in conjunction with the
   `jsPrintSetup <http://jsprintsetup.mozdev.org/>`__ Firefox add-on.
   Learn more about this preference and the add-on setup on the Koha
   wiki at
   http://wiki.koha-community.org/wiki/Setting_up_slip_printer_to_print_silently.

.. _intranetstylesheet-label:

intranetstylesheet
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Use the CSS stylesheet \_\_\_ on all pages in the staff interface,
instead of the default css (used when leaving this field blank).

Description:

-  The Intranetstylesheet preference is a layout and design feature for
   the intranet or staff client. This preference allows a library to
   customize the appearance of the Staff Client. Enter just a filename,
   a full local path or a complete URL starting with http:// (if the
   file lives on a remote server). Please note that if you just enter a
   filename, the file should be in the css subdirectory for each active
   theme and language within the Koha templates directory. A full local
   path is expected to start from your HTTP document root.

.. _intranetusercss-label:

IntranetUserCSS
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Include the following CSS on all pages in the staff client

.. _intranetuserjs-label:

IntranetUserJS
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Include the following JavaScript on all pages in the staff
interface

Description:

-  This preference allows the administrator to enter JavaScript or
   JQuery that will be embedded across all pages of the staff client.
   Administrators may use this preference to customize some of the
   interactive sections of Koha, customizing the text for the login
   prompts, for example. Sample JQuery scripts used by Koha libraries
   can be found on the wiki:
   http://wiki.koha-community.org/wiki/JQuery_Library.

.. _slipcss-label:

SlipCSS
^^^^^^^^^^^^^^^^^^^^^^

Asks: Include the stylesheet at \_\_\_ on Issue and Reserve Slips.

    **Important**

    This should be a complete URL, starting with http://

Description:

-  If you would like to style your receipts or slips with a consistent
   set of fonts and colors you can use this preference to point Koha to
   a stylesheet specifically for your slips.

.. _staffclientbaseurl-label:

staffClientBaseURL
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: The staff client is located at \_\_\_

    **Important**

    This should be a complete URL, starting with http:// or https://.
    Do not include a trailing slash in the URL.

    **Note**

    This must be filled in correctly for CAS, svc, and load_testing to work.

.. _stafflangselectormode-label:

StaffLangSelectorMode
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: only footer

Asks: Display language selector on \_\_\_

Values:

-  both top and footer

-  only footer

-  top

.. _stafflogininstructions-label:

StaffLoginInstructions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Show the following HTML on the staff client login page

Description:

-  HTML entered in this field will appear above the login form
   of your staff client

|image1345|

.. _template-label:

template
^^^^^^^^^^^^^^^^^^^^^^^^

Default: prog

Asks: Use the \_\_\_ theme on the staff interface.

Values:

-  prog

    **Important**

    Do not include a trailing slash in the URL this will break links
    created using this URL. (example: www.google.com not
    www.google.com/)

.. _xsltdetailsdisplay-label:

XSLTDetailsDisplay
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: default

Asks: Display details in the staff client using XSLT stylesheet at
\_\_\_

Values:

-  leave empty to not use the XSLT stylesheet

   -  In previous versions of Koha this was the setting that read
      'normally'

      |image119|

-  enter "default" for the default one

   |image120|

-  put a path to define a XSLT file

   -  ex: /path/to/koha/and/your/stylesheet.xsl

   -  If in a multi-language system you can enter {langcode} in the path
      to tell Koha to look in the right language folder

      -  ex:
         /home/koha/src/koha-tmpl/intranet-tmpl/prog/{langcode}/xslt/intranetDetail.xsl

      -  ex. http://mykoha.org/{langcode}/stylesheet.xsl

-  put an URL for an external specific stylesheet

   -  ex: http://mykoha.org/stylesheet.xsl

Description:

-  XSLT stylesheets allow for the customization of the details shown on
   the screen when viewing a bib record. This preference will allow you
   either use the default look that comes with Koha or design your own
   stylesheet.

.. _xsltlistsdisplay-label:

XSLTListsDisplay
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: default

Asks: Display lists in the staff client using XSLT stylesheet at
\_\_\_

Values:

-  leave empty to not use the XSLT stylesheet

   -  In previous versions of Koha this was the setting that read
      'normally'

-  enter "default" for the default one

-  put a path to define a XSLT file

   -  ex: /path/to/koha/and/your/stylesheet.xsl

   -  If in a multi-language system you can enter {langcode} in the path
      to tell Koha to look in the right language folder

      -  ex:
         /home/koha/src/koha-tmpl/intranet-tmpl/prog/{langcode}/xslt/intranetDetail.xsl

      -  ex. http://mykoha.org/{langcode}/stylesheet.xsl

-  put an URL for an external specific stylesheet

   -  ex: http://mykoha.org/stylesheet.xsl

Description:

-  XSLT stylesheets allow for the customization of the details shown on
   the screen when viewing a list. This preference will allow you
   either use the default look that comes with Koha or design your own
   stylesheet.

.. _xsltresultsdisplay-label:

XSLTResultsDisplay
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: default

Asks: Display results in the staff client using XSLT stylesheet at
\_\_\_

Values:

-  leave empty to not use the XSLT stylesheet

   -  In previous versions of Koha this was the setting that read
      'normally'

-  enter "default" for the default one

-  put a path to define a XSLT file

   -  ex: /path/to/koha/and/your/stylesheet.xsl

   -  If in a multi-language system you can enter {langcode} in the path
      to tell Koha to look in the right language folder

      -  ex:
         /home/koha/src/koha-tmpl/intranet-tmpl/prog/{langcode}/xslt/intranetDetail.xsl

      -  ex. http://mykoha.org/{langcode}/stylesheet.xsl

-  put an URL for an external specific stylesheet

   -  ex: http://mykoha.org/stylesheet.xsl

Description:

-  XSLT stylesheets allow for the customization of the details shown on
   the screen when viewing the search results. This preference will
   allow you either use the default look that comes with Koha or design
   your own stylesheet.

.. _options-label:

Options
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. _audioalerts-label:

AudioAlerts
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: Don't enable

Asks: \_\_\_ audio alerts for events defined in the audio alerts section
of administration.

Values:

-  Don't enable

-  Enable

    **Important**

    This feature is not supported by all browsers. Requires an HTML5
    compliant browser.

.. _hidepatronname-label:

HidePatronName
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: Show

Asks: \_\_\_ the names of patrons that have items checked out or on hold
on detail pages or the "Place Hold" screen.

Values:

-  Don't show

-  Show

.. _intranetbookbag-label:

intranetbookbag
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: Show

Asks: \_\_\_ the cart option in the staff client.

Values:

-  Don't show

-  Show

.. _intranetcatalogsearchpulldown-label:

IntranetCatalogSearchPulldown
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: Don't show

Asks: \_\_\_ a search field pulldown for 'Search the catalog' boxes.

Values:

-  Don't show

-  Show

.. _showLastPatron-label:

showLastPatron
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: Don't Show

Asks: \_\_\_ a link to the last searched patron in the staff client.

Values:

-  Don't show

-  Show

Description

- If this preference is set to 'Show' then a link to the last patron account
  you consulted will appear in the right hand corner of the Koha staff client.
  This link will be cleared when you log out.

  |image1423|

.. _staffdetailitemselection-label:

StaffDetailItemSelection
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: Enable

Asks: \_\_\_ item selection in record detail page.

Values:

-  Disable

-  Enable

Description:

-  This preference lets you choose to show (or not show) checkboxes to
   the left of every item in the holdings tab on the detail display of a
   record in the staff client. Showing these checkboxes allows the staff
   members to select multiple items to edit or delete at once.

   |image121|

.. _usewysiwyginsystempreferences-label:

UseWYSIWYGinSystemPreferences
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: \_\_\_ WYSIWYG editor when editing certain HTML system
preferences.

Default: Don't show

Values:

-  Don't show

-  Show

    |image1200|

Description:

-  This preference allows you to change system preferences with HTML in
   them to WYSIWYG editors instead of plain text boxes.

.. _viewisbd-label:

viewISBD
^^^^^^^^^^^^^^^^^^^^^^^^

Default: Allow

Asks: \_\_\_ staff to view records in ISBD form on the staff client.

Values:

-  Allow

-  Don't allow

.. _viewlabeledmarc-label:

viewLabeledMARC
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: Allow

Asks: \_\_\_ staff to view records in labeled MARC form on the staff
client.

Values:

-  Allow

-  Don't allow

.. _viewmarc-label:

viewMARC
^^^^^^^^^^^^^^^^^^^^^^^^

Default: Allow

Asks: \_\_\_ staff to view records in plain MARC form on the staff
client.

Values:

-  Allow

-  Don't allow


