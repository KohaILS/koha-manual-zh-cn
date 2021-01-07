.. include:: images.rst

.. _tools-system-preferences-label:

Tools
-----------------------

*Get there:* More > Administration > Global System Preferences > Tools

.. _barcodes-label:

Barcodes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. _barcodeseparators-label:

BarcodeSeparators
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: \\s\\r\\n

Asks: Split barcodes on the following separator chars \_\_\_ in batch item
modification and inventory.

Description:

-  When importing barcode files in the :ref:`inventory tool <inventory-tool-label>`
   or the :ref:`batch item modification tool <batch-item-modification-label>`
   you can decide which character separates each barcode.

   **Important**

   You must use the regular expression codes for the characters.

   -  \\s is used for a whitespace

   -  \\r is used for a carriage return

   -  \\n is used for a new line

   -  \\t is used for a tab

   Make sure you escape the other characters you put in there by preceding
   them with a backslash

   -  \\. instead of a dot

   -  \\\ instead of a backslash

   -  \\- instead of a hyphen

.. _batch-item-label:

Batch item
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

These preferences are in reference to the :ref:`Batch item
modification <batch-item-modification-label>` and :ref:`Batch item deletion
<batch-item-deletion-label>` tools.

.. _maxitemstodisplayforbatchdel-label:

MaxItemsToDisplayForBatchDel
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: 1000

Asks: Display up to \_\_\_ items in a single item deletion batch.

Description:

-  In the :ref:`batch item delete tool <batch-item-deletion-label>` this will
   prevent the display of more than the items you entered in this
   preference, but you will be able to delete more than the number you
   enter here.

.. _maxitemstodisplayforbatchmod-label:

MaxItemsToDisplayForBatchMod
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: 1000

Asks: Display up to \_\_\_ items in a single item modification batch.

Description:

-  In the :ref:`batch item modification tool <batch-item-modification-label>`
   this will prevent the display of more than the items you entered in this
   preference, but you will be able to modify more than the number you
   enter here (see :ref:`MaxItemsToProcessForBatchMod`).

.. _maxitemsforbatchmod-label:

MaxItemsToProcessForBatchMod
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: 1000

Asks: Process up to \_\_\_ items in a single modification batch.

Description:

-  In the :ref:`batch item modification
   tool <batch-item-modification-label>` this preference will prevent the editing
   of more than the number entered here.

.. _news-system-preferences-label:

News
~~~~~~~~~~~~~~~~~~~~~~~~~

.. _newsauthordisplay-label:

NewsAuthorDisplay
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: not at all

Asks: Show the author for news items: \_\_\_

Values:

-  Both OPAC and staff client

-  Not at all

-  OPAC only

-  Staff client only

.. _newstooleditor-label:

NewsToolEditor
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: By default edit news items with

Default: a WYSIWYG editor (TinyMCE)

Values:

-  a text editor (CodeMirror)

-  a WYSIWYG editor (TinyMCE)

Description:

-  This system preference allows you to choose which editor to use in the 
   :ref:`news tool <news-label>`.

-  A text editor will let you write HTML directly. Use this if you want more 
   control over how your content will be displayed. 

   **Note**

   You can use CSS id's and classes in your HTML and format them with the 
   :ref:`OPACUserCSS` system preference.

-  A WYSIWYG (what you see is what you get) editor is a user-friendly editor 
   with functions similar to word processing software. Use this if you are 
   unfamiliar with HTML.

.. _patron-cards-label:

Patron Cards
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

These preferences are in reference to the :ref:`Patron Card
Creator <patron-card-creator-label>` tool.

.. _imagelimit-label:

ImageLimit
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Limit the number of creator images stored in the database to
\_\_\_ images.

.. _reports-system-preferences-label:

Reports
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

These preferences are in reference to the Reports module.

.. _numsavedreports-label:

NumSavedReports
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: 20

Asks: By default, show \_\_\_ reports on the Saved Reports page.

.. _upload-system-preferences-label:

Upload
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. _uploadpurgetemporaryfilesdays-label:

UploadPurgeTemporaryFilesDays
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: blank

Asks: Automatically delete temporary uploads older than \_\_\_ days in
cleanup_database cron job.


