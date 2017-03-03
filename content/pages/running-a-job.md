Title: Running a Job
url: running-a-job
save_as: running-a-job.html
section: runningajob
index: 2

Running a Job
==========

How to run a Job

------

After unpacking a Arrebol release package (listed here), the Arrebol CLI script can be found in bin/directory.
To submit a JDF-formatted job, run the arrebol script with the POST command:
`bin/arrebol.sh POST jdf_file_path -u [username]`
It is mandatory to specify the path of the JDF-formatted file which describes the job and a username for indentification, you will then be asked a password. On sucessful execution, the bin/arrebol.sh script outputs a unique identifier to the submitted job.
To retrieve status information about all running jobs, run the arrebol script with the GET command:
`bash bin/arrebol.sh GET -u [username]`
To retrieve information about a specific running job, run the arrebol script witht GET and specify the job id or the the job friendly name.
`bash bin/arrebol.sh GET [job id or friendly name] -u [username]`
To stop a running job, run the arrebol script with the STOP command with the associated job id or friendly name.
`bash arrebol.sh STOP [job id or friendly name] -u [username]`

in all cases you will be asked to submit a password



