**DAY 1 Introduction to SoC Design Flow and Synthesis:**

![image](https://github.com/user-attachments/assets/a47db024-433e-4926-98b6-f743a4dcf45b)
Opening openlane & design preparation:
![image](https://github.com/user-attachments/assets/f8bd1246-daf1-4369-8bbd-3f6fd5d5639d)

Run Synthesis:
![image](https://github.com/user-attachments/assets/421f06a6-7525-43a6-8dfc-1b158c3ac192)


**DAY 2 Floorplan and Placement:**

Runninf floorplan:
![image](https://github.com/user-attachments/assets/731876a7-fbee-4f0b-aa5f-5ebd9da52d66)

Opening floorplan def on magic:
![image](https://github.com/user-attachments/assets/b6f43324-85df-4f95-bf5a-37ee1205b868)

![image](https://github.com/user-attachments/assets/412a8f89-77d2-48a5-a93d-8071935a70b7)

Running Placement:
![image](https://github.com/user-attachments/assets/eb82bce8-0d26-443f-aa89-7bde1f8e8358)

Opening placement def on magic:
![image](https://github.com/user-attachments/assets/b1700868-9010-470b-ba0b-3058d57c32b5)
![image](https://github.com/user-attachments/assets/3f053858-ad96-40f0-a05c-9f8cde75efa5)

**Day3 Design of Inverter:**

Cloning the inverter cell from the Github repository:
![image](https://github.com/user-attachments/assets/2dea9edc-7bc9-46ca-afbc-2bda66f2838a)

Opening inverter layout:
![image](https://github.com/user-attachments/assets/986a90c0-2336-42d7-b8a7-6c7035485079)
![image](https://github.com/user-attachments/assets/462bc20c-37bf-4327-95ad-dbb8a73eba5c)

Extracting the inverter & creating spice file:
![image](https://github.com/user-attachments/assets/305866d0-0f8d-426d-a5e8-c3c927d860e1)
![image](https://github.com/user-attachments/assets/e2729f8e-f7d1-47bc-ae92-2eeffa68a459)

Spice Simulation:
![image](https://github.com/user-attachments/assets/dd7702ff-3a02-46d3-b82e-626211f6a0e3)
![image](https://github.com/user-attachments/assets/4091feb3-deaa-4395-8d33-3abe87fd899b)

Updated A, Y, VPWR & VGND definitions and saved the lef of my inverter.
![image](https://github.com/user-attachments/assets/7d0dfd70-e504-4d29-a840-0d6226b89054)

Opened the lef & checked the PIN definitions.
![image](https://github.com/user-attachments/assets/2ab2fb12-aec7-4207-9094-ad842aa714fd)
![image](https://github.com/user-attachments/assets/f34206b3-3a60-4d5b-9282-0392efb2ff96)


**DRC correction and rules:**

![image](https://github.com/user-attachments/assets/90796dcb-ef60-4063-9324-fe50c91d61d3)
![image](https://github.com/user-attachments/assets/6c05b416-9691-4d86-97e5-ba14a0071026)
![image](https://github.com/user-attachments/assets/be9f1edc-9736-42e9-ab2b-f567aaf6f35a)

Metal 3 DRC rules in tech file.

![image](https://github.com/user-attachments/assets/582c0f14-bc06-4e5a-8f3c-989a30ca70dd)

Updating the Metal 3 DRC rules in tech file as below:

![image](https://github.com/user-attachments/assets/31728b16-0a0e-4d29-833d-17424643c37e)

Reduced the Min width from 0.3um to 0.003um

Now, met3.1 ERROR was resolved.
![image](https://github.com/user-attachments/assets/41f1c8e3-0b39-4517-b4d4-f0c377f5d351)


**Day 4 - Prelayout design and Clock Tree Synthesis**

Copied all the libs & newly created lef of the inverter cell into src for picorv design directory.
![image](https://github.com/user-attachments/assets/759b2b7e-417e-4a08-a52f-399632458a10)

![image](https://github.com/user-attachments/assets/627fd1cc-dea6-424c-9c53-f436c00dee45)

Then, updated config.tcl below:
![image](https://github.com/user-attachments/assets/a9c6bc8f-d20b-458e-bad5-31873981b1ef)

With updated config file (added inverter libs), prep design command was performed again:
![image](https://github.com/user-attachments/assets/f7e4e41e-f92e-4d86-a68d-a3049cadad77)

Performed synthesis again after adding our inverter cell.
![image](https://github.com/user-attachments/assets/4a6d7652-0da7-4108-ad6e-88778c985a8f)

Done till placement again.
![image](https://github.com/user-attachments/assets/1d3faf04-1b36-415f-8761-5968f70db137)

Performed run_cts :
![image](https://github.com/user-attachments/assets/165c3856-a2f3-4cb8-aca3-e0a9245b4e54)

**Day 5 - PDN & Routing**

**PDN**

Performed gen_pdn:
![image](https://github.com/user-attachments/assets/11fc5bfa-8300-4ca8-93c3-3d023fb75406)
![image](https://github.com/user-attachments/assets/c03904a0-88c8-4657-b3b8-2ad1cebc2ff6)

Performed run_routing:
![image](https://github.com/user-attachments/assets/8a777ca6-872f-4642-ab1c-172e7b955944)


**Certificate of Completion from VLSI Sytem Design:**

![image](https://github.com/user-attachments/assets/ecc9ac64-d2b4-42b2-929a-e2f9b3212af0)
