******************
cinq-scheduler-sqs
******************

===========
Description
===========

This scheduler takes caree of the scheduling the actual SQS 
messaging and tracks the status of the jobs as workers are 
executing said jobs.

Please check out the `README <https://github.com/RiotGames/cloud-inquisitor/blob/master/docs/backend/README.rst>`_ 
for further details on the how ``cinq-scheduler-sqs`` works with 
further details on ``Cloud Inquisitor`` backend is built and what 
technologies we use.

=====================
Configuration Options
=====================

+---------------------+--------------------------------------+--------+------------------------------------------------------------------------------------------------------------+
| Option name         | Default Value                        | Type   | Description                                                                                                |
+=====================+======================================+========+============================================================================================================+
| enabled             | False                                | bool   | Enable SQS based scheduler                                                                                 |
+---------------------+--------------------------------------+--------+------------------------------------------------------------------------------------------------------------+
| queue_region        | us-west-2                            | string | Region of the SQS Queues                                                                                   |
+---------------------+--------------------------------------+--------+------------------------------------------------------------------------------------------------------------+
| status_queue_url    |                                      | string | URL of the SQS Queue for worker reports                                                                    |
+---------------------+--------------------------------------+--------+------------------------------------------------------------------------------------------------------------+
| job_delay           | 2                                    | float  | Time between each scheduled job, in seconds. Can be used to avoid spiky loads during execution of tasks    |
+---------------------+--------------------------------------+--------+------------------------------------------------------------------------------------------------------------+
