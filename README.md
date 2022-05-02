# VASP_submitscript
This submit script allows me to streamline my calculations. I am still working on having the geometry optimization loop stop once the convergence criteria is met & the single point energy calculations starting. Currently, I have not been able to get the calculation to kick out of the geometry optimization loop once the convergence criteria is met. 

Also, this script does not correctly calculate the updated MAGMOM if the job doesn't finish. For example, if my job was kicked out of the cluster for some unknown reason, the OUTCAR file isn't written to completion. Most likely those lines associated with the magnetization won't be written either. Meaning the lines the script reads is incorrect. I have started using a python script from another scientist that calculates the magnetization. I have that scipt uploaded under the Python repository.

Will update this with the job submit script I am currently using at a later date.
