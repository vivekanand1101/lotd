* Open multiple connections for the http request.
* Run each connections in a different thread
* Each connection will download from different bytes
* Join the output of each thread

    The Server has to accept 'range' header in order for this method to work.
    Source: http://stackoverflow.com/a/1798945/3181759
    and: http://stackoverflow.com/a/13973531/3181759
