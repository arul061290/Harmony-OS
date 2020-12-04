Development Guidelines on Animators
===================================

When to Use
-----------

A UI animator is implemented by calling the callback function you set
for each tick using the task processing mechanism. The following classes
are provided for you to implement an animator:

-  **AnimatorManager**: Manages Animator instances. This is a singleton
   class, which is registered with the system task callback when the
   **Init** function is executed. The system task mechanism ensures that
   each tick invokes the callback function of **AnimatorManager**.
-  **Animator**: Represents animator-related attributes, including the
   start and end time of an animator. It also provides animator-specific
   functions, for example, to start and stop an animator, to set the
   animator state, and to obtain the animator.
-  **AnimatorCallback**: Implements the content of each tick. You need
   to implement your own logic in this callback class so that the
   desired operation is executed upon the corresponding callback is
   invoked.

Available APIs
--------------

**Table 1** Available functions for an animator

.. raw:: html

   <table>

.. raw:: html

   <thead align="left">

.. raw:: html

   <tr id="row1389130182514">

.. raw:: html

   <th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.4.1.1">

.. raw:: html

   <p id="p16390130172517">

Module

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="54.13%" id="mcps1.2.4.1.2">

.. raw:: html

   <p id="p239060112519">

Function

.. raw:: html

   </p>

.. raw:: html

   </th>

.. raw:: html

   <th class="cellrowborder" valign="top" width="28.52%" id="mcps1.2.4.1.3">

.. raw:: html

   <p id="p1839012019257">

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

   <tr id="row1533075412415">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p633015547249">

Animator

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p6330554152411">

void Start ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p3330155472412">

Starts an animator.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18330175410241">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p33301454172415">

Animator

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p12330195419248">

void Stop ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p23301854162416">

Stops the animator.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row433045420244">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p183301054182410">

Animator

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p43302054172415">

void Pause ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p15330854182413">

Pauses the animator.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1033085492417">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p12331135413244">

Animator

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p5331165472412">

void Resume ()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p63314543246">

Resumes the animator.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row1331175413240">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p18331454152418">

Animator

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p15331155472414">

uint8_t GetState () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p2033125414243">

Obtains the current state of the animator.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row43311554182415">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p33311854172420">

Animator

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p433165462418">

void SetState (uint8_t state)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p23316546242">

Sets the current state for the animator.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row17331254192419">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p173319547243">

Animator

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p18332125416243">

uint32_t GetTime () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p1633295412414">

Obtains the total duration of the animator.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row8332195419241">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2033211545243">

Animator

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p123321054172415">

void SetTime (uint32_t time)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p4332105472411">

Sets the total duration for the animator.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row13332125412420">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p17332165482417">

Animator

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p3332115417243">

uint32_t GetRunTime () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p733275442419">

Obtains the running time of the animator.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row2033215419249">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p113327549245">

Animator

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p43321154172417">

void SetRunTime (uint32_t runTime)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p173331354182416">

Sets the running time for the animator.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row20333115417249">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p2333155412240">

Animator

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p143335549246">

bool IsRepeat () const

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p23336548244">

Checks whether the animator is repeated.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row19333754202418">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1833319543247">

AnimatorCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p6333135402416">

virtual void Callback (UIView \*view)=0

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p19333854172417">

Represents the animator callback. You can implement your own logic in
this callback.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row193331854112415">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p1133325482420">

AnimatorCallback

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p1433585412411">

virtual void OnStop(UIView& view) {}

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p933595412249">

Called after the animator stops. You can implement your own logic in
this callback.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row83351654192415">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p633525419244">

AnimatorManager

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p203351547242">

static AnimatorManager\* GetInstance()

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p333545412419">

Obtains an AnimatorManager instance.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row3335954202412">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p5335185413247">

AnimatorManager

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p11336145442417">

void Add (Animator \*animator)

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p10336175492416">

Adds an animator.

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   </tr>

.. raw:: html

   <tr id="row18336185422417">

.. raw:: html

   <td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.4.1.1 ">

.. raw:: html

   <p id="p103361554192411">

AnimatorManager

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="54.13%" headers="mcps1.2.4.1.2 ">

.. raw:: html

   <p id="p6336195442412">

void Remove(const Animator\* animator);

.. raw:: html

   </p>

.. raw:: html

   </td>

.. raw:: html

   <td class="cellrowborder" valign="top" width="28.52%" headers="mcps1.2.4.1.3 ">

.. raw:: html

   <p id="p233615442420">

Removes the animator.

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

1. Implement the callback in **AnimatorCallback**.

   ::

      class AnimatorCallbackDemo : public OHOS::AnimatorCallback {
      public:
          AnimatorCallbackDemo(int16_t startPos, int16_t endPos, uint16_t time)
              : start_(startPos), end_(endPos), time_(time), curTime_(0) {}

          virtual void Callback(OHOS::UIView* view)
          {
              curTime_++;
              int16_t pos = EasingEquation::CubicEaseIn(start_, end_, curTime_, time_);
              view->Invalidate();
              view->SetPosition(pos, view->GetY());
              view->Invalidate();
          }
      protected:
          int16_t start_;
          int16_t end_;
          uint16_t time_;
          uint16_t curTime_;
      };

2. Register **AnimatorCallback** to the animator.

   ::

      UIImageView* image = new UIImageView();
      image->SetSrc("..\\config\\images\\A021_001.bin");
      image->SetPosition(0, 50);
      AnimatorCallbackDemo* callback = new AnimatorCallbackDemo(0, 338, 60);
      Animator* animator = new Animator(callback, image, 0, true);

3. Add the animator to **AnimatorManager**.

   ::

      AnimatorManager::GetInstance()->Add(animator);

4. Click the buttons in the lower part of the following figure to verify
   that the animation effects are as expected.

   | **Figure 1** Animator effect
   | |image1|

.. |image1| image:: figures/animator-effect.gif
