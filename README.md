# CPU-SIM-PRACTICAL
In this practical we will be creating multiple things using Hardware Modules and Microinstructions :

1. Base Machine :
   
   To create our Base Machine we will first open Cpusim4.bat
   
   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/6113a812-4bbb-4246-980e-75027a3ae289" />
   
   The interface will look like this.

   Now we will make a New Text File in it using the File Menu at the top left corner.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/e354071f-d1ef-4fff-97d5-7e1f44444ce4" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/84d97038-e85a-4db8-962b-8f8d310cdee6" />

   As we can see our New Text File is created successfully and it is completely blank.
   So, now we will create a New Machine using the same File Menu as before.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/abb839d9-dbc7-43bc-bd4a-93d5af1346fa" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/45426761-2ff0-4705-a318-3022ef3609a7" />

   As we can see now our New Machine is also created successfully and currently has no content.

   1.1. Now we will be moving towards creating Hardware Modules :
       To create Hardware Modules we will go to Modify Menu at the top left corner.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/b152a20f-90c7-4202-8bb1-5cf316481dfe" />

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/176fc71c-bb45-41f8-9e9b-cc21d836a904" />

         As we can see we are now inside Hardware Modules and moving towards creating RAM and Registers.
         1.1.1. Creating RAM (MAIN) :
                  To create RAM we will go to Types of Modules which is at the top.
                 
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
               2. HALT-BIT      -->    Register = S, TICK HALT

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

      Now we will change Indexing for Instruction Format because indexing is done from the left side.
         To change Indexing we will go to Execute at the top left corner and click on Options.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/ec0461dc-f4e5-40f2-910a-f1a29bdfbf03" />

         Then click on Indexing and select Left.

   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/a2a92c66-b603-4a2a-b490-91b699d6accb" />

         And click on OK.
   
   <img width="1440" height="900" alt="image" src="https://github.com/user-attachments/assets/54a6f083-059b-4c46-9198-c4e14b468e6a" />

















