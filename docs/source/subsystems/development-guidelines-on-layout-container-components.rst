Development Guidelines on Layout Container Components
=====================================================

Layout container components consist of basic view classes. You can set
the view positions to achieve nested and overlapped layouts, set the
layout type and margin to standardize the child components in the
layout, and call certain functions to implement layout views based on
parent and sibling components.

UISwipeView
-----------

When to Use
-----------

**UISwipeView** inherits from **UIViewGroup**. In addition to the
**Add**, **Remove**, and **Insert** functions, **UISwipeView** provides
the functions to swipe contents by page and center the current page
after swiping. This component can be horizontally or vertically
centered. Child components added via the **Add** function are
automatically horizontally or vertically centered, adaptive to the
**UISwipeView** direction, in the sequence they were added.

Available APIs
--------------

**Table 1** Available functions in SwipeView

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row8336122032615">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p13361520162611">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p153361920112617">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   </tr>

.. raw:: html

   </thead>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row9336720172616">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p83365206267">

void SetCurrentPage(uint16_t index);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1833612017261">

Sets the current page.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row15336172002613">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p0336162072613">

uint16_t GetCurrentPage()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p433615207262">

Obtains the current page.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row9336920102614">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p6336520102619">

UIView\* GetCurrentView() const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p16336112062612">

Obtains the current view.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row03371820162616">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p7336172082611">

void SetOnSwipeListener(OnSwipeListener& onSwipeListener)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p15336172012269">

Sets the swiping callback class.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row23371520172613">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p733792017267">

void SetAnimatorTime(uint16_t time);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p16337112012613">

Sets the animator event.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row12337152011269">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p9337220152610">

void SetLoopState(bool loop)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p12337172032612">

Sets whether to enable the cyclic state.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1033713201266">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p1933792092610">

UIView\* GetViewByIndex(uint16_t index);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p033714208263">

Obtains a view based on its index.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

Development Procedure (Non-Cyclic Horizontal Swiping)
-----------------------------------------------------

1. Create a horizontal swiping **UISwipeView**.

   ::

      UISwipeView* swipe = new UISwipeView(UISwipeView::HORIZONTAL);

2. Add child components to **UISwipeView**.

   ::

      UILabelButton* button1 = new UILabelButton();
      button1->SetPosition(0, 0, g_ButtonW, g_ButtonH);
      button1->SetText("button1");
      swipe->Add(button1);
      UILabelButton* button2 = new UILabelButton();
      button2->SetPosition(0, 0, g_ButtonW, g_ButtonH);
      button2->SetText("button2");
      swipe->Add(button2);
      UILabelButton* button3 = new UILabelButton();
      button3->SetPosition(0, 0, g_ButtonW, g_ButtonH);
      button3->SetText("button3");
      swipe->Add(button3);

3. Verify that the components are swiping horizontally but not
   cyclically.

   **Figure 1** Horizontal swiping effect of **UISwipeView**\ 

   |image1|

Development Procedure (Cyclic Horizontal Swiping)
-------------------------------------------------

1. Create a horizontal swiping **UISwipeView** and add its child
   components.

   ::

      UISwipeView* swipe = new UISwipeView(UISwipeView::HORIZONTAL);
      UILabelButton* button1 = new UILabelButton();
      button1->SetPosition(0, 0, g_ButtonW, g_ButtonH);
      button1->SetText("button1");
      swipe->Add(button1);
      UILabelButton* button2 = new UILabelButton();
      button2->SetPosition(0, 0, g_ButtonW, g_ButtonH);
      button2->SetText("button2");
      swipe->Add(button2);
      UILabelButton* button3 = new UILabelButton();
      button3->SetPosition(0, 0, g_ButtonW, g_ButtonH);
      button3->SetText("button3");
      swipe->Add(button3);

2. Enable cyclic swiping for the **UISwipeView**.

   ::

      swipe->SetLoopState(true);

3. Verify that the components are swiping horizontally and cyclically.

   **Figure 2** Cyclic horizontal swiping effect of **UISwipeView**\ 

   |image2|

GridLayout
----------

.. _when-to-use-1:

When to Use
-----------

**GridLayout** provides the basic layout capability to set the number of
grid rows and columns. Child components added via the **Add** function
are automatically arranged after the **LayoutChildren()** function is
called.

.. _available-apis-1:

Available APIs
--------------

**Table 2** Available functions in GridLayout

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row9997104632911">

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1">

.. raw:: html

   <p id="p119971146192917">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2">

.. raw:: html

   <p id="p7997204615291">

Description

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   </tr>

.. raw:: html

   </thead>

.. raw:: html

   <tbody>

.. raw:: html

   <tr id="row149976467292">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p159971046102912">

void SetRows(const uint16_t& rows)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p14997846132913">

Sets the number of grid rows.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row299774652915">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p099744615296">

void SetCols(const uint16_t& cols)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p19971646142910">

Sets the number of grid columns.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1199724616291">

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 ">

.. raw:: html

   <p id="p18997846202912">

void LayoutChildren(bool needInvalidate = false)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 ">

.. raw:: html

   <p id="p1997174618291">

Lays out child components.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   </tbody>

.. raw:: html

   </table>

How to Develop
--------------

1. Create a **GridLayout** instance and set its position and size.

   ::

      GridLayout* layout_ = new GridLayout();
      layout_->SetPosition(0, g_y, HROIZONTAL_RESOLUTION, 200);
      layout_->SetLayoutDirection(LAYOUT_HOR);
      layout_->SetRows(2);
      layout_->SetCols(2);

2. Create **UILabelButton** instances.

   ::

      UILabelButton* bt1 = new UILabelButton();
      bt1->SetPosition(0,0,100,50);
      bt1->SetText("bt1");
      UILabelButton* bt2 = new UILabelButton();
      bt2->SetPosition(0, 0, 100, 50);
      bt2->SetText("bt2");
      UILabelButton* bt3 = new UILabelButton();
      bt3->SetPosition(0, 0, 100, 50);
      bt3->SetText("bt3");
      UILabelButton* bt4 = new UILabelButton();
      bt4->SetPosition(0, 0, 100, 50);
      bt4->SetText("bt4");

3. Add child components and call the **LayoutChildren()** function.

   ::

      layout_->Add(bt1);
      layout_->Add(bt2);
      layout_->Add(bt3);
      layout_->Add(bt4);
      layout_->LayoutChildren();

4. Verify the layout of buttons, as shown in the following figure.

   | **Figure 3** Setting a 2x2 grid and adding four buttons in a layout
   | |image3|

.. |image1| image:: figures/en-us_image_0000001053247975.gif
.. |image2| image:: figures/en-us_image_0000001053207924.gif
.. |image3| image:: figures/setting-a-2x2-grid-and-adding-four-buttons-in-a-layout.png
