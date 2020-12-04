GPIO Usage Guidelines
=====================

How to Use
----------

The GPIO APIs use the GPIO pin number to specify a pin. `Figure
1 <#fig1399416053717>`__ shows the general process of using a GPIO.

| **Figure 1** Process of using a GPIO
| |image1|

Determining a GPIO Pin Number
-----------------------------

The method for converting GPIO pin numbers varies according to the GPIO
controller model, parameters, and controller driver of different system
on chips (SoCs).

-  Hi3516D V300

   A controller manages 12 groups of GPIO pins. Each group contains 8
   GPIO pins.

   GPIO pin number = GPIO group index (0-11) x Number of GPIO pins in
   each group (8) + Offset in the group

   Example: GPIO number of GPIO10_3 = 10 x 8 + 3 = 83

-  Hi3518E V300

   A controller manages 10 groups of GPIO pins. Each group contains 10
   GPIO pins.

   GPIO pin number = GPIO group index (0–9) x Number of GPIO pins in
   each group (10) + Offset in the group

   Example: GPIO pin number of GPIO7_3 = 7 x 10 + 3 = 73

Using APIs to Operate GPIO Pins
-------------------------------

-  Set the direction for a GPIO pin.

   Before performing read/write operations on a GPIO pin, call the
   following function to set the direction:

   int32_t GpioSetDir(uint16_t gpio, uint16_t dir);

   **Table 1** Description of GpioSetDir

   .. raw:: html

      <table>

   .. raw:: html

      <tbody>

   .. raw:: html

      <tr id="row17311165469">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p53110515616">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p5311454616">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row0312151666">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p1431265763">

   gpio

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p83121553613">

   GPIO pin number.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row11312151619">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p173121451664">

   dir

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p153122520615">

   Direction to set.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row165937126386">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p83111453613">

   Return Value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p83111151165">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row205931212123817">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p18312151463">

   0

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p103124517618">

   The setting is successful.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row75931212153818">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p23121951261">

   Negative value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p153121553610">

   The setting failed.

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

-  Read or write the level value for a GPIO pin.

   To read the level value of a GPIO pin, call the following function:

   int32_t GpioRead(uint16_t gpio, uint16_t \*val);

   **Table 2** Description of GpioRead

   .. raw:: html

      <table>

   .. raw:: html

      <tbody>

   .. raw:: html

      <tr id="row17348144394816">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p19348164313481">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p134810432488">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row134874324814">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p183481437485">

   gpio

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p43481043194819">

   GPIO pin number.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row20348343144815">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p1534864310480">

   val

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p13689159154815">

   Pointer to the level value.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row19348043154813">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p1234812431480">

   Return Value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p434894334814">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row3348184311486">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p1934854315487">

   0

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p103481943114814">

   Succeeded in reading the level value.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row23485436482">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p1134834310486">

   Negative value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p93491343144815">

   Failed to read the level value.

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

   To write the level value for a GPIO pin, call the following function:

   int32_t GpioWrite(uint16_t gpio, uint16_t val);

   **Table 3** Description of GpioWrite

   .. raw:: html

      <table>

   .. raw:: html

      <tbody>

   .. raw:: html

      <tr id="row6149720175218">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p18149132005216">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p16149220145216">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row16149102014526">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p31495206527">

   gpio

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p1014972085212">

   GPIO pin number.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row3149112095214">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p1815072011528">

   val

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p1931618337524">

   Level value to write.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1115062015220">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p10150172015218">

   Return Value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p1150192015527">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row111503202526">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p171501320205216">

   0

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p15150102017522">

   Succeeded in writing the level value.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1615002018528">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.120000000000005%">

   .. raw:: html

      <p id="p15150182045212">

   Negative value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.88%">

   .. raw:: html

      <p id="p13150320105212">

   Failed to write the level value.

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

   Example:

   ::

      int32_t ret;
      uint16_t val;
      /* Set the output direction for GPIO3. */
      ret = GpioSetDir(3, GPIO_DIR_OUT);
      if (ret != 0) {
          HDF_LOGE("GpioSerDir: failed, ret %d\n", ret);
          return;
      }
      /* Write the low level GPIO_VAL_LOW for GPIO3. */
      ret = GpioWrite(3, GPIO_VAL_LOW);
      if (ret != 0) {
          HDF_LOGE("GpioWrite: failed, ret %d\n", ret);
          return;
      }
      /* Set the input direction for GPIO6. */
      ret = GpioSetDir(6, GPIO_DIR_IN);
      if (ret != 0) {
          HDF_LOGE("GpioSetDir: failed, ret %d\n", ret);
          return;
      }
      /* Read the level value of GPIO6. */
      ret = GpioRead(6, &val);

-  Set the ISR function for a GPIO pin.

   To set the ISR function for a GPIO pin, call the following function:

   int32_t GpioSetIrq(uint16_t gpio, uint16_t mode, GpioIrqFunc func,
   void \*arg);

   **Table 4** Description of GpioSetIrq

   .. raw:: html

      <table>

   .. raw:: html

      <tbody>

   .. raw:: html

      <tr id="row880401834615">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.54%">

   .. raw:: html

      <p id="p380491819469">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.459999999999994%">

   .. raw:: html

      <p id="p48041318114619">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row19805181812465">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.54%">

   .. raw:: html

      <p id="p11805101874611">

   gpio

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.459999999999994%">

   .. raw:: html

      <p id="p6805181818461">

   GPIO pin number.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1080541817469">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.54%">

   .. raw:: html

      <p id="p580541864611">

   mode

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.459999999999994%">

   .. raw:: html

      <p id="p380511180463">

   Interrupt trigger mode.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row83541951134617">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.54%">

   .. raw:: html

      <p id="p5355351104610">

   func

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.459999999999994%">

   .. raw:: html

      <p id="p11355551174619">

   ISR function to set.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row6593577469">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.54%">

   .. raw:: html

      <p id="p165985724619">

   arg

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.459999999999994%">

   .. raw:: html

      <p id="p559185784619">

   Pointer to the parameters passed to the ISR function.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row16299193210587">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.54%">

   .. raw:: html

      <p id="p7804101884614">

   Return Value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.459999999999994%">

   .. raw:: html

      <p id="p680441818466">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row12299632125817">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.54%">

   .. raw:: html

      <p id="p1180511189465">

   0

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.459999999999994%">

   .. raw:: html

      <p id="p180521812465">

   The setting is successful.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row029833235815">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.54%">

   .. raw:: html

      <p id="p1080591814468">

   Negative value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.459999999999994%">

   .. raw:: html

      <p id="p18805141884611">

   The setting failed.

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

   ..

      |image2| **CAUTION:** Only one ISR function can be set for a GPIO
      pin at a time. If **GpioSetIrq** is called repeatedly, the
      previous IRS function will be replaced.

   If the ISR function is no longer required, call the following
   function to cancel the setting:

   int32_t GpioUnSetIrq(uint16_t gpio);

   **Table 5** Description of GpioUnSetIrq

   .. raw:: html

      <table>

   .. raw:: html

      <tbody>

   .. raw:: html

      <tr id="row175721546174317">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.54%">

   .. raw:: html

      <p id="p16572144694311">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.459999999999994%">

   .. raw:: html

      <p id="p185721461435">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1257284664318">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.54%">

   .. raw:: html

      <p id="p95721946144317">

   gpio

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.459999999999994%">

   .. raw:: html

      <p id="p1557313464439">

   GPIO pin number.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1857324618435">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.54%">

   .. raw:: html

      <p id="p1257344624314">

   Return Value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.459999999999994%">

   .. raw:: html

      <p id="p457384611439">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row357318466439">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.54%">

   .. raw:: html

      <p id="p1573164616438">

   0

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.459999999999994%">

   .. raw:: html

      <p id="p857384614319">

   The ISR function is canceled.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row18573124610433">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="48.54%">

   .. raw:: html

      <p id="p165731146134311">

   Negative value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="51.459999999999994%">

   .. raw:: html

      <p id="p6573164613437">

   Failed to cancel the ISR function.

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

   After the ISR function is set, call the following function to enable
   a GPIO interrupt:

   int32_t GpioEnableIrq(uint16_t gpio);

   **Table 6** Description of GpioEnableIrq

   .. raw:: html

      <table>

   .. raw:: html

      <tbody>

   .. raw:: html

      <tr id="row866632919566">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p066642985615">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p566613293568">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row19666029165620">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p16660295566">

   gpio

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p1566632916566">

   GPIO pin number.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row84182176010">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p1566652915566">

   Return Value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p966642917562">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row154188171403">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p1866610292563">

   0

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p13666182975613">

   The GPIO interrupt is enabled.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row1041891720012">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p766642911562">

   Negative value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p1566652995613">

   Failed to enable a GPIO interrupt.

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

   ..

      |image3| **CAUTION:** The configured ISR function can be responded
      only after the ISR function is enabled.

   Use the following function to disable the GPIO interrupt:

   int32_t GpioDisableIrq(uint16_t gpio);

   **Table 7** Description of GpioDisableIrq

   .. raw:: html

      <table>

   .. raw:: html

      <tbody>

   .. raw:: html

      <tr id="row186684413116">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p866844916">

   Parameter

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p46681413119">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row4668243113">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p46681141919">

   gpio

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p136681241311">

   GPIO pin number.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row066884412">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p566824015">

   Return Value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p1766974515">

   Description

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row156694410112">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p14669141214">

   0

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p1266934818">

   The GPIO interrupt is disabled.

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      </tr>

   .. raw:: html

      <tr id="row176691543117">

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p7669941716">

   Negative value

   .. raw:: html

      </p>

   .. raw:: html

      </td>

   .. raw:: html

      <td class="cellrowborder" valign="top" width="50%">

   .. raw:: html

      <p id="p4669164219">

   Failed to disable the GPIO interrupt.

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

   Example:

   ::

      /* ISR function */
      */
      int32_t MyCallBackFunc(uint16_t gpio, void *data)
      {
          HDF_LOGI("%s: gpio:%u interrupt service in! data=%p\n", __func__, gpio, data);
          return 0;
      }

      int32_t ret;
      /* Set the ISR function to MyCallBackFunc, the parameter to NULL, and the interrupt trigger mode to rising edge. */
      ret = GpioSetIrq(3, OSAL_IRQF_TRIGGER_RISING, MyCallBackFunc, NULL);
      if (ret != 0) {
          HDF_LOGE("GpioSetIrq: failed, ret %d\n", ret);
          return;
      }

      /* Enable an interrupt for GPIO3. */
      ret = GpioEnableIrq(3);
      if (ret != 0) {
          HDF_LOGE("GpioEnableIrq: failed, ret %d\n", ret);
          return;
      }

      /* Disable the interrupt for GPIO3. */
      ret = GpioDisableIrq(3);
      if (ret != 0) {
          HDF_LOGE("GpioDisableIrq: failed, ret %d\n", ret);
          return;
      }

      /* Cancel the ISR function for GPIO3. */
      ret = GpioUnSetIrq(3);
      if (ret != 0) {
          HDF_LOGE("GpioUnSetIrq: failed, ret %d\n", ret);
          return;
      }

.. |image1| image:: figures/process-of-using-a-gpio.png
.. |image2| image:: public_sys-resources/icon-caution.gif
.. |image3| image:: public_sys-resources/icon-caution.gif
