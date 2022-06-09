## Prerequisites
* Docker

## Basic Setup
1. Create a folder where you want the data of Photoprism to be saved, for example "D:/Photoprism"
2. Get the latest "docker-compose.yml" from [Setup Using Docker Compose](https://docs.photoprism.app/getting-started/docker-compose/)
3. Paste/Save "docker-compose.yml" in the newly created directory "D:/Photoprism"

![2022-06-09 04_41_58-Photoprism](https://user-images.githubusercontent.com/7150376/172752818-894b76f0-64b6-47c9-a1ab-00bb28b23355.png)

4. Edit the "docker-compose.yml" to your liking. Recommended changes:
* PHOTOPRISM_ADMIN_PASSWORD: "insecure" > PHOTOPRISM_ADMIN_PASSWORD: "YOURPASSWORD"
* PHOTOPRISM_ORIGINALS_LIMIT: 5000 > PHOTOPRISM_ORIGINALS_LIMIT: 50000
* PHOTOPRISM_JPEG_QUALITY: 85 > PHOTOPRISM_JPEG_QUALITY: 100

5. Open the folder with Windows Terminal

![2022-06-09 04_46_22-Greenshot](https://user-images.githubusercontent.com/7150376/172753447-24ed52fd-5ea1-4455-b114-bfbd8e06a2c0.png)

6. Copy paste "docker-compose up -d" and press Enter

![2022-06-09 04_58_59-Windows PowerShell](https://user-images.githubusercontent.com/7150376/172754859-3d678b63-ace1-403e-aafa-00506c975c86.png)

## Additional
* To add new/other folders for import/storage you'll have to add them to "volumes"

![2022-06-09 05_03_18-D__Photoprism_docker-compose yml - Notepad++](https://user-images.githubusercontent.com/7150376/172755373-b2c8ece6-604d-4c48-9121-d2c6ac06df72.png)

**Important:** Keep in mind that "photoprism/originals", "photoprism/storage" and "photoprism/import" are used as a variable, the pictures will be saved under "User/Pictures" **not** "User/Pictures/photoprism/originals"!

For additonal info about the folder structure see [Setup Using Docker Compose](https://docs.photoprism.app/getting-started/docker-compose/).

* You can use the "Import" function to import complete folders.
* To delete pictures you'll have to archieve them first.

## Unsolved Questions
* How do i backup data?
* What can i add to docker-compose.yml?
