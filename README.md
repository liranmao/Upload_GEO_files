# Upload_GEO_files


Here is a tuotorial about how to upload the files to GEO for publication.

Please check the [**Submitting high-throughput sequence data to GEO**](https://www.ncbi.nlm.nih.gov/geo/info/seq.html)

1. Finish step1-step4 and step6.
2. Step5 is not neccessary.
3. For step7, click the link and it will lead you to login in or creat an account. After finish creating the account, the page is like this:
   <img width="749" alt="image" src="https://github.com/liranmao/Upload_GEO_files/assets/78578236/7483d068-9987-4e74-a922-1b89f8ea0899">

  Then, click Transfer Files, you will see FTP server credentials in f.

  Edit run.lftp file accordingly and put it in the parent directory. 
  
  Use this comand to run the code: nohup lftp -f ../run.lftp > ../run.lftp.out &

  You can check if there are errors in run.lftp.out file.

  
5. Upload the metadata. For setting the release date, you can just set 1 or 2 years. This can be eddited afterwards. 
6. After the submission, you will be redirct to a conformation page and received a conformation email as well. Also, expect to receive an email from GEO curators with your GEO accession numbers, or questions about your submission. 


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

3. **Upload the metadata.** When setting the release date, a general guideline is to choose a date 1 or 2 years from the present. This can be adjusted later if necessary.
4. Upon completing your submission, you will be directed to a confirmation page and will receive a confirmation email. Additionally, expect an email from GEO curators containing your GEO accession numbers or posing questions regarding your submission.
