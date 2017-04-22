Readme on INT Sample Code
HL 

1. This sample code EXTINT-2016-11-28.zip is provided for reference only, 
   it demonstrate how GPIO port configured for EXTINT handling. You can 
   use Xpresso IDE to create a new project then import this zip 
   project file. To do so, you want to first create a C simehost project, 
   then import LPC1769 patch first, once it is done, then you can 
   import this sample project. 

2. Once this project imported, go to src folder to locate extint.c code, 
   you can browse the "uint32_t EINTInit( void )" module to inspect the 
   code for external EINT initialization and configuration; and "void 
   EINT1_IRQHandler (void)" (ISR, interrupt service routine, e.g., user written
   program to realize specific interrupt functions. Note how the interrupt type
   (number), "NVIC_EnableIRQ(EINT1_IRQn);" is connected to the ISR program 
   "void EINT1_IRQHandler (void)" .   

(END) 
