# CSA-CPU-SIM-PRACTICAL
In this practical we will be creating multiple things using Hardware Modules and Microinstructions :

1. Base Machine :
   
   To create our Base Machine we will first open Cpusim4.bat
   
   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/6113a812-4bbb-4246-980e-75027a3ae289" />
   
   The interface will look like this.

   Now we will make a New Text File in it using the File Menu at the top left corner and clicking on New Text.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/e354071f-d1ef-4fff-97d5-7e1f44444ce4" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/84d97038-e85a-4db8-962b-8f8d310cdee6" />

   As we can see our New Text File is created successfully and it is completely blank.
   So, now we will create a New Machine using the same File Menu as before.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/abb839d9-dbc7-43bc-bd4a-93d5af1346fa" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/45426761-2ff0-4705-a318-3022ef3609a7" />

   As we can see now our New Machine is also created successfully and currently has no content.

   1.1. Now we will be moving towards creating Hardware Modules :
       To create Hardware Modules we will go to Modify Menu at the top left corner and click on Hardware Modules.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/b152a20f-90c7-4202-8bb1-5cf316481dfe" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/176fc71c-bb45-41f8-9e9b-cc21d836a904" />

         As we can see we are now inside Hardware Modules and moving towards creating RAM and Registers.
         1.1.1. Creating RAM (MAIN) :
                  To create RAM we will go to Types of Modules which is at the top and select RAM.
                 
   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/cdf74b7b-95a4-46a7-8b21-5ecd36dca42b" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/d6550f64-0ef7-42e6-9819-b9f5a1e54c80" />

                  Now we will create RAM called RAM (MAIN) of size 4096 X 8 using NEW at the bottom left.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/08e640da-c9d7-402d-9845-216f0b2a7675" />

                  As we can see our RAM is created successfully.
         1.1.2. Creating Registers :
                  We will create register same way as we created RAM.

                  There are many kinds of registers but what we will be creating today are :

                  1. PC (Program Counter)       -->    Width = 12 bits
                  2. AR (Address Register)      -->    Width = 12 bits
                  3. IR (Instruction Register)  -->    Width = 16 bits
                  4. AC (Accumulator)           -->    Width = 16 bits
                  5. DR (Data Register)         -->    Width = 16 bits
                  6. E (CARRY-BIT)              -->    Width = 1 bits
                  7. S (Status Register)        -->    Width = 1 bits
                  8. I (Direct/Indirect)        -->    Width = 1 bits

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/ac65f77e-caf0-402a-9da7-b29bf8846e4f" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/95a9dd70-5862-4a90-91d7-a5d60f2d57ff" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/6fa90fbc-ed36-472c-8fab-ef74af41c05e" />

                  As we can see our Registers is created successfully.

         1.1.3. Creating Condition Bit :
                  We will create Condition Bit same way as we created Registers.   

               There are many kinds of Condition Bit but what we will be creating today are :

               1. CARRY-BIT     -->    Register = E
               2. HALT-BIT      -->    Register = S | TICK HALT

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/e9db6ebe-5379-4695-9fb0-8b402060c19a" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/8c3a9e36-2198-4f39-afcc-f5237d8b3ccc" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/5a195e3c-d529-4008-92c9-becf055fce7e" />

               As we can see our Condition Bit is created successfully.

      We will click OK now and as we can see everything we created is showing up.
   
   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/98c9610b-0022-4f16-8ce2-07de00d289a1" />

      Now we are going to click on Save Machine, and save our file as .cpu extension using File Menu at the top left.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/1df198ff-b739-4358-b9cf-9b1973fb2ba7" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/e8e8d014-772e-4018-9b75-142f2fbcefab" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/d2451cb4-37e3-4306-85a6-416e28e31204" />

   1.2. Now we will be moving towards creating Microinstructions :
         To create Microinstruction we will go to Modify Menu at the top left corner and click on Microinstructions.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/eb15cca6-f2c5-4694-99da-0ddd4974a34f" />

         1.2.1. Creating TransferRtoR Microinstructions :
                  To create TransferRtoR we will go to Types of Microinstructions which is at the top.
                  We will create Microinstructions using New.

                  There are many kinds of TransferRtoR Microinstructions but what we will be creating today are :

                  1. PC --> AR       | Source = PC | srcStarBit = 0 | Dest = AR | numBits = 12
                  2. IR(4-15) --> AR | Source = PC | srcStarBit =0  | Dest = AR | numBits = 12

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/5384a7ea-89fe-4a33-bfaa-b5ecb208e5d0" />

         1.2.2. Creating MemoryAccess Microinstructions :
                  To create we will do same as TransferRtoR and select MemoryAccess this time.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/84a4e276-428e-4b6e-afcf-156c642badcc" />

                  There are many kinds of MemoryAccess Microinstructions but what we will be creating today is :

                  1. AR[MAIN] --> IR | Memory = RAM(MAIN) | Data = IR | Address = AR

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/5a42bb20-a592-4ed2-86fd-dfba75526231" />

         1.2.3. Creating Increment Microinstructions :
                  To create we will do same as MemoryAccess and select Increment this time.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/9944a07e-4826-4caf-b14d-2306da79f3e5" />

                  There are many kinds of Increment Microinstructions but what we will be creating today is :

                  1. INCR - PC | Register = PC | Delta = 1

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/ebeb982f-e05d-43a8-af14-84d764f7e42d" />

         1.2.4. Creating Decode Microinstructions :
                  To create we will do same as Increment and select Decode this time

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/7f2f68d2-4ee8-4f2b-9e32-8a36612a6c68" />

                  There are many kinds of Decode Microinstructions but what we will be creating today is :

                  1. DECODE - IR | IR = IR

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/378c12c2-3715-4c0a-ba97-255c376406b9" />

      Now we will simply click on OK.

   1.3. Now we will be moving towards creating Fetch Sequence :
         To create Fetch Sequence we will go to Modify Menu at the top left corner and click on Fetch Sequence.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/3a8a317e-b00c-46f2-b70c-3534e9c5c68e" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/43c3b884-cb48-43cd-ad6e-e30ecb584ae5" />

         1. We will go to TransferRtoR and fetch PC --> AR by drag and drop.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/4c5b4ded-7a54-497a-9fa3-f27545159346" />

         2. We will go to Memory and fetch AR[MAIN] --> IR by drag and drop.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/b7f5ecbd-0a4b-4273-9980-f5459c63237e" />

         3. We will go to Increment and fetch INCR - PC by drag and drop.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/5012ef1f-3eb7-45ab-8d8b-3a823cfa50db" />

         4. We will go to TransferRtoR and fetch IR(4-15) --> AR by drag and drop.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/83d15bf2-8e37-4444-bd8d-1d5ca7df6077" />

         5. We will go to Decode and fetch DECODE - IR by drag and drop.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/a619c0ee-6a18-4556-be2e-c694bdc8befd" />
      Now we will simply click on OK.
   
   1.4. Now we will be moving towards creating Machine Instructions :
         To create Machine Instructions we will go to Modify Menu at the top left corner and click on Machine Instruction.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/381bb20a-9b2d-44a7-bda2-0775a2b7d9fb" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/88605738-8c5e-4277-92af-7131ceda286f" />

         1.4.1. Now we will create Field using Edit Field :
   
   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/3f2f2c51-95f6-4d76-b126-a46df0b8ae5c" />

                  There are different types of Fields but what we will be creating today is :

                  1. OP       | Type = required | NumBits = 4  | Signed = Unsigned
                  2. ADDR     | Type = required | NumBits = 12 | Signed = Unsigned
                  3. REGISTER | Type = required | NumBits = 16 | Signed = Unsigned

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/979ae292-7e25-41e5-b5df-afe0263ebd2d" />
   
            Now we will simply click on OK.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/64d3d920-4fbf-4707-beb9-a0cfb47595e3" />

            Saving everything we did by Ctrl+B




















