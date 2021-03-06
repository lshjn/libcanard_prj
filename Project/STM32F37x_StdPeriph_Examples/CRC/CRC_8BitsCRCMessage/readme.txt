/**
  @page CRC_8BitsCRCMessage Compute the 8-bit CRC value of a message
  
  @verbatim
  ******************** (C) COPYRIGHT 2012 STMicroelectronics *******************
  * @file    CRC/CRC_8BitsCRCMessage/readme.txt 
  * @author  MCD Application Team
  * @version V1.0.0
  * @date    20-September-2012
  * @brief   Description of the 8-bit CRC value of a message example.
  ******************************************************************************
  *
  * Licensed under MCD-ST Liberty SW License Agreement V2, (the "License");
  * You may not use this file except in compliance with the License.
  * You may obtain a copy of the License at:
  *
  *        http://www.st.com/software_license_agreement_liberty_v2
  *
  * Unless required by applicable law or agreed to in writing, software 
  * distributed under the License is distributed on an "AS IS" BASIS, 
  * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  * See the License for the specific language governing permissions and
  * limitations under the License.
  *
  ******************************************************************************
  @endverbatim

@par Example Description 

This example aims to show how to use the CRC peripheral in order to compute
8-bit CRC checksum of a message.
The CRC peripheral is configured to use the 8-bit CRC polynomial x8 + x7 + x6 + x4 + x2 + 1 
with the initialization value set to 0.
The message is declared as an array and labeled "CRCBuffer".
The expected CRC value is already computed using an on line CRC tool.
Once the CRC value is computed, the computed CRC value is compared to the expected
one. In case of match the green led LD1 is turned on. Otherwise the led LD3 is turned on.


@par Directory contents 

  - CRC/CRC_8BitsCRCMessage/stm32f37x_conf.h    Library Configuration file
  - CRC/CRC_8BitsCRCMessage/stm32f37x_it.c      Interrupt handlers
  - CRC/CRC_8BitsCRCMessage/stm32f37x_it.h      Interrupt handlers header file
  - CRC/CRC_8BitsCRCMessage/main.c              Main program
  - CRC/CRC_8BitsCRCMessage/system_stm32f37x.c  STM32F37x system source file
  
@note The "system_stm32f37x.c" is generated by an automatic clock configuration 
      system and can be easily customized to your own configuration. 
      To select different clock setup, use the "STM32F37x_Clock_Configuration_V1.0.0.xls" 
      provided with the AN4132 package available on <a href="http://www.st.com/internet/mcu/family/141.jsp">  ST Microcontrollers </a>
         
@par Hardware and Software environment

  - This example runs on STM32F37x Devices.
  
  - This example has been tested with STMicroelectronics STM32373C-EVAL (STM32F37x)
    evaluation board and can be easily tailored to any other supported device 
    and development board.


@par How to use it ? 

In order to make the program work, you must do the following :
 - Copy all source files from this example folder to the template folder under
   Project\STM32F37x_StdPeriph_Templates
 - Open your preferred toolchain 
 - Rebuild all files and load your image into target memory
 - Run the example

 * <h3><center>&copy; COPYRIGHT STMicroelectronics</center></h3>
 */
