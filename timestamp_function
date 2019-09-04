from datetime import datetime
from time import gmtime, strftime


de get_current_gmt_time():
    """
    This functions gives the current utc time.
    Format of out - 2019-08-29T10:55:29.Z where UTC is 0.
    Note: you will not get the values of miliseconds part.
    """
    return str(strftime("%Y-%m-%dT%H:%M:%S.Z", gmtime()))
    
def time_diff_in_seconds(timestamp_1, timestamp_2):
    """
    This function calcultes the time difference between two different 
    time. The imput time stamp should look like - 2019-08-29T10:55:29.511782712Z
    input data type: string

    :param time_1: before time
    :param time_2: after time
    :return: the time difference in seconds
    Note: Output will be in seconds precision, cannot be used for getting output
          milliseconds.
    """
    
    timestamp_1 = timestamp_1.split('.')[0]
    timestamp_2 = timestamp_2.split('.')[0]
    time_format = '%Y-%m-%dT%H:%M:%S'
    
    formated_time_1 = datetime.strptime(timestamp_1, time_format)
    formated_time_2 = datetime.strptime(timestamp_2, time_format)
    return (formated_time_1-formated_time_1).seconds
