# Maximo Mobile Certificate Installation

## Download the certificate file
1. Access the Maximo Application Suite server page in your browser on a desktop computer. A message indicates that the connection is not private.
    1. On Firefox, click the ```Advanced``` -> ```view certificate``` link to open the certificate in a new tab
        1. <img width="3456" height="2234" alt="image" src="https://github.com/user-attachments/assets/553b9b5b-079e-49e8-8afa-440f360986fe" />


2. Find and save the certificate of the root certificate authority.
    1. On Safari, click to view the certificate, select the root certificate, and drag the file to a folder.
    2. On Firefox, click the ```public.mas.mas.ibm.com``` tab then scroll to ```Miscellaneous``` -> and click  ```PEM (cert)``` to download the Root CA certificate for the server
        1. <img width="3456" height="2234" alt="image" src="https://github.com/user-attachments/assets/e227a10f-3446-48cf-9d30-7600f004ed40" />
        2. <img width="3456" height="2234" alt="image" src="https://github.com/user-attachments/assets/4949d8b8-bc2c-4a3e-b84c-45cab234283e" />


## Install the certificate profile
1. Use Airdrop to send the saved root certificate file to your iOS device.
    1. <img width="450" alt="image" src="https://github.com/user-attachments/assets/079fecf5-9ef3-4c74-9ef9-4b79fbc340cc" />
    2. <img width="300" alt="image" src="https://github.com/user-attachments/assets/82e3f157-5a39-40f8-b100-83b3970e7eaa" />

2. Open the Device Settings page.
3. In the User details section of the device settings, click Profile Downloaded.
    1. <img width="300" alt="image" src="https://github.com/user-attachments/assets/85d67a9b-1277-44ad-83dd-2904fbe1b577" />

5. In the Install Profile page, click Install.
    1. <img width="300" alt="image" src="https://github.com/user-attachments/assets/2a263629-007d-4c2f-af07-839afa3897a3" />

7. If you are prompted, enter the iOS device passcode. A certificate warning is displayed.
8. Click Install and click Install again if you are prompted.
9. On the Profile Installed page, click Done.

## Trust the certificate
1. On the device, go to Settings > General > About > Certificate Trust Settings. The installed root certificate is displayed in the Enable Full Trust for Root Certificates.
2. Turn on trust for the certificate that you installed and click Continue. The certificate is trusted and enabled and you can proceed to use the Maximo Mobile application.
    1. <img width="300" alt="image" src="https://github.com/user-attachments/assets/a22bbadf-a591-4e9d-a19f-20a5a79c4c3f" />


## Congrats! Now you can open up the Maximo Mobile App

1. Server URL (Scan from the IBM Maximo Mobile App)
    1. <img width="250" alt="image" src="https://github.com/user-attachments/assets/663bbaca-3939-412c-ac99-17050eb5a6a4" />

 
