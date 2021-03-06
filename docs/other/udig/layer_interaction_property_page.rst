Layer Interaction Property Page
###############################

uDig : Layer Interaction Property Page

This page last changed on Nov 23, 2011 by jgarnett.

Motivation
----------

The layer data model allows developers greater programmatic control of layer / tool interaction than
is currently made available to the users.

This page proposes to "out" a very interesting ability of the Layer model - control of how Layers
and Tools interact.

Inspiration
-----------

Inspiration comes from the layer properties pages and in a similar way to the Projection page allows
the layer to be configured for display.

User stories:

-  "applicability" bits are present in the application and we don't have a preference page to allow
   users to change them.
-  The "applicability" bits are used to control how the layer interacts with Tools
-  The normal applicability bit is "visible"; and that is the one displayed in the layer list.
-  The usual GIS use case is to hide a layer (visible = false) but still allow "info" tool to select
   from it (info = "true"). This allows GIS professionals to work with large datasets that may be
   too slow to draw.
-  By the same fashion you can turn (visible=false, edit=true) and edit data you cannot see :-P
-  The use case that is interesting me today is the mark "background" layers so that they don't take
   part in the normal tool relationships (hopefully we can look into rendering them into tiles or
   something later).
-  The immediate follow up to this is the use of a `Boundary Selection
   Tool <Boundary%20Selection%20Tool.html>`__ (which makes use of background layers as a source of
   "boundary" polygons which can be used to filter map contents)

Default Vector
~~~~~~~~~~~~~~

|image0|

Raster
~~~~~~

| |image1|
|   

 Polygon
~~~~~~~~

| |image2|
|   
|   
|   

Proposal
--------

Add an layer preference page that displays if a layer is:

-  Visible
-  Select
-  Edit
-  Information (ie a "Query" request)
-  Boundary

Status
------

Project Steering committee support:

-  Andrea Antonello: +0 (indicated enthusiasm but not vote)
-  Jesse Eichar: +0
-  Jody Garnett: +1
-  Mauricio Pazos: +1

Committer Support:

-   

A vote of -1 requires an alternate suggestion; community members are invited to indicate
support/suggestions.

Documentation
-------------

Documentation change to `Users Guide <http://udig.refractions.net/confluence//display/EN/Home>`__
(for an accepted change).

Tasks
=====

A list of the tasks needed to accomplish this change; if you prefer you can use a single Jira issue
with subtasks. It is important to include any deadlines so the community knows when you are working
to a schedule.

 

no progress

|image3|

in progress

|image4|

blocked

|image5|

help needed

|image6|

done

Tasks:

#. |image7| Initial interface wireframe for community review and feedback
#. |image8| Review from PSC member required
#. Initial implementation in git fork
#. Code Review
#. Updated user guide documentation
#. Pull Request

Status:

-  https://jira.codehaus.org/browse/UDIG-1825

| 

Attachments:

| |image9| `LayerPreferences.screen <download/attachments/13534009/LayerPreferences.screen>`__
(application/octet-stream)
|  |image10| `LayerPreferences.png <download/attachments/13534009/LayerPreferences.png>`__
(image/png)
|  |image11|
`RasterLayerInteraction.screen <download/attachments/13534009/RasterLayerInteraction.screen>`__
(application/octet-stream)
|  |image12|
`RasterLayerInteraction.png <download/attachments/13534009/RasterLayerInteraction.png>`__
(image/png)
|  |image13| `LayerInteraction.screen <download/attachments/13534009/LayerInteraction.screen>`__
(application/octet-stream)
|  |image14| `LayerInteraction.png <download/attachments/13534009/LayerInteraction.png>`__
(image/png)
|  |image15|
`PolygonLayerInteraction.screen <download/attachments/13534009/PolygonLayerInteraction.screen>`__
(application/octet-stream)
|  |image16|
`PolygonLayerInteraction.png <download/attachments/13534009/PolygonLayerInteraction.png>`__
(image/png)

+-------------+----------------------------------------------------------+
| |image18|   | Document generated by Confluence on Aug 11, 2014 12:31   |
+-------------+----------------------------------------------------------+

.. |image0| image:: /images/layer_interaction_property_page/LayerInteraction.png
.. |image1| image:: /images/layer_interaction_property_page/RasterLayerInteraction.png
.. |image2| image:: /images/layer_interaction_property_page/PolygonLayerInteraction.png
.. |image3| image:: images/icons/emoticons/star_yellow.gif
.. |image4| image:: images/icons/emoticons/error.gif
.. |image5| image:: images/icons/emoticons/warning.gif
.. |image6| image:: images/icons/emoticons/check.gif
.. |image7| image:: images/icons/emoticons/check.gif
.. |image8| image:: images/icons/emoticons/warning.gif
.. |image9| image:: images/icons/bullet_blue.gif
.. |image10| image:: images/icons/bullet_blue.gif
.. |image11| image:: images/icons/bullet_blue.gif
.. |image12| image:: images/icons/bullet_blue.gif
.. |image13| image:: images/icons/bullet_blue.gif
.. |image14| image:: images/icons/bullet_blue.gif
.. |image15| image:: images/icons/bullet_blue.gif
.. |image16| image:: images/icons/bullet_blue.gif
.. |image17| image:: images/border/spacer.gif
.. |image18| image:: images/border/spacer.gif
