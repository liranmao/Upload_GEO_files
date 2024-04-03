# Upload Files to GEO

This tutorial guides you through the process of uploading files to GEO for publication.

Please refer to [**Submitting high-throughput sequence data to GEO**](https://www.ncbi.nlm.nih.gov/geo/info/seq.html) for detailed instructions.

## Steps for Submission

1. Complete **Steps 1 to 4** and **Step 6** as outlined in the guide. Step 5 is optional and not necessary for this process.
2. For **Step 7**, follow the provided link to either log in to your existing account or create a new one. Upon successful account creation or login, you will encounter a screen similar to the following:

    <img width="749" alt="image" src="https://github.com/liranmao/Upload_GEO_files/assets/78578236/7483d068-9987-4e74-a922-1b89f8ea0899">

    Next, select **Transfer Files**. You will find the FTP server credentials displayed.

    Modify the `run.lftp` file as needed and place it in the parent directory. Execute the transfer with the following command:

    ```bash
    nohup lftp -f ../run.lftp > ../run.lftp.out &
    ```

    Check the `run.lftp.out` file for any errors that may have occurred during the transfer.

3. Upload the metadata. Note that when setting the release date, a general guideline is to choose a date 1 or 2 years from the present. This can be adjusted later if necessary.
4. Upon completing your submission, you will be directed to a confirmation page and will receive a confirmation email. Additionally, expect an email from GEO curators containing your GEO accession numbers or posing questions regarding your submission.
