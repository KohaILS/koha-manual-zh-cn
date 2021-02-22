.. include:: images.rst

.. _acquisitions-system-preferences-label:

Acquisitions
-------------------------------------------------------------------------------

*Get there:* More > Administration > Global system preferences > Acquisitions

.. _acquisitions-edifact-system-preferences-label:

EDIFACT
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. _edifactinvoiceimport-label:

EdifactInvoiceImport 
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: \_\_\_ automatically import EDIFACT invoice message files when they are 
downloaded. 

Default: Do

Values:

-  Do

-  Don't

.. _acquisitions-policy-label:

Policy
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. _acqcreateitem-label:

AcqCreateItem
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Create an item when \_\_\_.

Default: placing an order

Values:

-  cataloging a record

-  placing an order

-  receiving an order

Description:

-  This preference lets you decide when you'd like to create an item record in 
   Koha. 

-  If you choose to add an item record when 'placing an order', you will enter 
   item information in as you :ref:`add records in your basket <create-a-basket-label>`. 

-  If you choose to add the item when 'receiving an order' you will be asked 
   for item record information when you're :ref:`receiving orders <receiving-orders-label>` 
   in acquisitions.

-  If you choose to add the item when 'cataloging a record' then item records 
   will not be created in acquisitions at all. You will need to go to the 
   :ref:`cataloging module <cataloging-label>` to
   :ref:`add the items <adding-items-label>`.

-  Note that this setting can be overridden when 
   :ref:`creating a basket <create-a-basket-label>`.

.. _acqenablefiles-label:

AcqEnableFiles
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: \_\_\_ enable the ability to upload and attach arbitrary files to
invoices.

Default: Don't

Values:

-  Do

-  Don't

Description:

-  This preference controls whether or not you allow the 
   :ref:`uploading of invoice files <attaching-files-to-invoices-label>` via 
   the acquisitions module.

.. _acqitemsetsubfieldswhenreceiptiscancelled-label:

AcqItemSetSubfieldsWhenReceiptIsCancelled
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Upon cancelling a receipt, update the item's subfields if they
were created when placing an order (e.g. o=5\|a="bar foo""). \_\_\_

Description:

-  This preference is used in conjunction with the
   :ref:`AcqItemSetSubfieldsWhenReceived`
   preference. If you have the system set to enter default values when
   you receive you will want to have those values revert back if the
   receipt is cancelled. This preference allows you to do that.

.. _acqitemsetsubfieldswhenreceived-label:

AcqItemSetSubfieldsWhenReceived
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Upon receiving items, update their subfields if they were created
when placing an order (e.g. o=5\|a="foo bar"). \_\_\_

Description:

-  This preference allows you to set default values for items that you
   receive via acquisitions. Enter the data as subfield=value and split
   your values with a bar ( \| ). For example you can remove the Ordered
   status on the item automatically when you receive it just by entering
   7=0 in this preference. That will set the Not for Loan status
   (subfield 7) to 0 which is available.

.. _acqviewbaskets-label:

AcqViewBaskets
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: created by staff member

Asks: Show baskets \_\_\_

Values:

-  created by staff member

-  from staff member's branch

-  in system, regardless of owner

Description:

-  When in acquisitions this preference allows you to control whose
   baskets you can see when looking at a vendor. The default value of
   'created by staff member' makes it so that you only see the baskets
   you created. Choosing to see baskets 'from staff member's branch'
   will show you the baskets created by anyone at the branch you're
   logged in at. Finally, you can choose to set this preference to show
   you all baskets regardless of who created it ('in system, regardless
   of owner). Regardless of which value you choose for this preference,
   superlibrarians can see all baskets created in the system.

.. _acqwarnonduplicateinvoice-label:

AcqWarnOnDuplicateInvoice
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: Do not warn

Asks: \_\_\_ when the librarian tries to create an invoice with a
duplicate number.

Values:

-  Do not warn

-  Warn

.. _basketconfirmations-label:

BasketConfirmations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: always ask for confirmation

Asks: When closing or reopening a basket, \_\_\_.

Values:

-  always ask for confirmation

-  do not ask for confirmation

Descriptions:

-  This preference adds the option to skip confirmations on closing and
   reopening a basket. If you skip the confirmation, you do not create a
   new basket group.

.. _claimsbcccopy-label:

ClaimsBccCopy
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: Don't send

Asks: \_\_\_ blind copy (BCC) to logged in user when sending serial or
acquisitions claims notices.

Values:

-  Don't send

-  Send

Description:

-  When filing a claim in the :ref:`Claim Late Serials` or
   Acquisitions module this preference will allow for
   the sending of a copy of the email to the librarian.

.. _currencyformat-label:

CurrencyFormat
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: 360,000.00 (US)

Asks: Display currencies using the following format \_\_\_

Values:

-  360,000.00 (US)

-  360 000,00 (FR)

.. _taxrates-label:

TaxRates
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Tax rates are \_\_\_

Default: 0

Description:

-  This preference allows the library to define goods and services tax rates 
   for acquisitions.

-  The first item in the list will be selected by default.

.. Note ::

   Enter this value as a number (.06) versus a percent (6%).

   For more than one value, separate with \| (pipe).

   For example

   0|0.05|0.1496

   will give you choices of tax rates of 0%, 5% and 14.96%

.. Warning ::

   The database only accepts values up to 4 decimals, further values will be 
   rounded. 

.. _marcfieldstoorder-label:

MarcFieldsToOrder
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Set the mapping values for a new order line created from a MARC
record in a staged file.

Description:

-  This preference includes MARC fields to check for order information
   to use when you are trying to :ref:`Order from a staged file` in
   acquisitions. You can use the following fields: price, quantity,
   budget\_code, discount, sort1, sort2.

   For example:

   ::

       price: 947$a|947$c
       quantity: 969$h
       budget_code: 922$a

**Important**
Requires YAML syntax to work

.. _marcitemfieldstoorder-label:

MarcItemFieldsToOrder
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Set the mapping values for new item records created from a MARC record
in a staged file.

Description:

-  This preference automatically generates items in Koha with populated
   information based on a 9XX field and subfield. You can use the following
   fields: homebranch, holdingbranch, itype, nonpublic_note, public_note, loc,
   ccode, notforloan, uri, copyno, price, replacementprice and itemcallnumber.
   Special fields: quantity and budget_code

For example:

::

       homebranch: 975$a
       holdingbranch: 975$b
       public_note: 975$z
       loc: 975$c

**Requires YAML syntax to work**

.. _purgesuggestionsolderthan-label:

PurgeSuggestionsOlderThan
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Asks: Keep accepted or rejected purchase suggestions for a period of \_\_\_ days.

    **Important**

    WARNING - Leave this field empty if you don't want to activate this automatic feature.

Description:

-  Enter the number of days after which you want to automatically
   delete accepted or rejected purchase suggestions.

-  For example: [30] Sets purgation of suggestions for those older than 30 days.

    **Note**

    This system preference is used when the cronjob purge_suggestions.pl is
    active and called without a specific number of days.

.. _uniqueitemfields-label:

UniqueItemFields
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: barcode

Asks: The following database columns should be unique in an item: \_\_\_
separate columns with pipe (|).

Description:

-  If this preference is left blank when adding items in acquisitions
   there will be no check for uniqueness. This means that a duplicate
   barcode can be created in acquisitions which will cause errors later
   when checking items in and out.

.. _useacqframeworkforbibliorecords-label:

UseACQFrameworkForBiblioRecords
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: Don't use

Asks: \_\_\_ the framework 'ACQ' for bibliographic records fields

Values:

-  Don't use

-  Use

Description:

-  This system preference allows you to use the ACQ framework to customize
   the bibliographic record fields that are shown when ordering from acquisitions

.. _printing-label:

Printing
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. _orderpdfformat-label:

OrderPdfFormat
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Default: pdfformat::layout2pages

Asks: Use \_\_\_ when printing basket groups.
