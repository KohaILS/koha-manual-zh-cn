.. include:: images.rst

.. _serials-system-preferences-label:

Serials
---------------------------

*Get there:* More > Administration > Global System Preferences > Serials

.. _makepreviousserialavailable-label:

makePreviousSerialAvailable
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Default: Do not make

Asks: \_\_\_ previous serial automatically available when receiving a
new serial issue. The previous issue can also be set to another item
type when receiving a new one. Please note that the :ref:`item-level\_itypes <item-level\_itypes-label>`
syspref must be set to specific item.

Values:

-  Do not make

-  Make

.. _opacserialdefaulttab-label:

opacSerialDefaultTab
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Default: Subscriptions tab

Asks: Show \_\_\_ as default tab for serials in OPAC.

Values:

-  Holdings tab

-  Serial Collection tab

       **Important**

       Please note that the Serial Collection tab is currently available
       only for systems using the UNIMARC standard.

   |image109|

-  Subscriptions tab

   |image110|

.. _opacserialissuedisplaycount-label:

OPACSerialIssueDisplayCount
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Default: 3

Asks: Show the \_\_\_ previous issues of a serial on the OPAC.

Description:

-  This preference allows the administrator to select the number of
   recent issues for each serial which appear in the OPAC when the
   serial is accessed. This is just the default value, patrons can
   always click to see a full list of serials.

.. _renewserialaddssuggestion-label:

RenewSerialAddsSuggestion
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Default: Don't add

Asks: \_\_\_ a suggestion for a biblio when its attached serial is
renewed.

Values:

-  Add

-  Don't add

Description:

-  If set to "Add", this preference will automatically add a serial to
   the Acquisitions Purchase Suggestions menu when clicking the 'renew'
   option. If you don't use the Acquisitions module to manage serials
   purchases it's best to leave this set as 'Don't add.^

.. _routinglistaddreserves-label:

RoutingListAddReserves
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Default: Place

Asks: \_\_\_ received serials on hold if they are on a routing list.

Values:

-  Place

-  Don't place

.. _routinglistnote-label:

RoutingListNote
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Asks: Include following note on all routing lists

Description:

-  Text entered in this box will appear below the routing list
   information.

.. _routingserials-label:

RoutingSerials
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Default: Don't add

Asks: \_\_\_ received serials to the routing list.

Description:

-  This preference determines if serials routing lists are enabled or
   disabled for the library. When set to "Add", serials routing is
   enabled and a serial can be directed through a list of people by
   identifying who should receive it next. The list of people can be
   established for each serial to be passed using the Serials module.
   This preference can be used to ensure each person who needs to see a
   serial when it arrives at the library will get it. Learn more in the
   :ref:`routing list <create-a-routing-list-label>` section of this manual.

Values:

-  Add

-  Don't add

.. _staffserialissuedisplaycount-label:

StaffSerialIssueDisplayCount
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Default: 3

Asks: Show the \_\_\_ previous issues of a serial on the staff client.

Description:

-  This preference allows the administrator to select the number of
   recent issues for each serial which appear in the Staff Client when
   the serial is accessed. This is just the default value, staff members
   can always click to see a full list of serials.

.. _subscriptionduplicatedroppedinput-label:

SubscriptionDuplicateDroppedInput
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Asks: List of fields which must not be rewritten when a subscription is
duplicated (Separated by pipe \|) \_\_\_

Description:

-  When duplicating a subscription sometimes you don't want all of the
   fields duplicated, using this preference you can list the fields that
   you don't want to be duplicated. These field names come from the
   subscription table in the Koha database. Learn what fields are in
   that table on the `Koha DB
   Schema <http://schema.koha-community.org/master/tables/subscription.html>`__
   site.

.. _subscriptionhistory-label:

SubscriptionHistory
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Default: full history

Asks: When showing the subscription information for a bibliographic
record, preselect \_\_\_ view of serial issues.

Values:

-  brief history

   |image111|

-  full history

   |image112|

Description:

-  This preference determines what information appears in the OPAC when
   the user clicks the More Details option. The 'brief' option displays
   a one-line summary of the volume and issue numbers of all issues of
   that serial held by the library. The 'full' option displays a more
   detailed breakdown of issues per year, including information such as
   the issue date and the status of each issue.


