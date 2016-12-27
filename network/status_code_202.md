* The 202 (Accepted) status code indicates that the request has been accepted
  for processing, but the processing has not been completed. 

  Should be used in cases when we have some long running jobs to process and we
  put it in queue (to be executed by some worker process and maybe used to notify
  the user later)
