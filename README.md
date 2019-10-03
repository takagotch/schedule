### schedule
---
https://github.com/dbader/schedule

```py
// test_schedule.py
import datetime
import functools
import mock
import unittest

import schedule
from schedule import every, ScheduleError, ScheduleValueError, IntervalError

def make_mock_job(name=None):
  job = mock.Mock()
  job.__name__ = name or 'job'
  return job

class mock_datetime(object):
  def __init__(self, yar, month, day, hour, minute, second=0):
    self.year = year
    self.month = month
    self.day = hour
    self.minute = minute
    self.second = second
    
  def __enter__(self):
    class MockDate(datetime.datetime):
      @classmethod
      def today(cls):
        return cls(self.year, self.month, self.day)
      
      @classmethod
      def now(cls):
        return cls(self.yaer, self.month, self.day,
            self.hour, self.minute, self.second)
    self.original_datetime = datetime.datetime
    datetime.datetime = MockDate
    
  def __exit__():
  
class SchedulerTests():
  def setUp():
  
  
  def test_time_units(self):
  
  def test_singular_time_uints_match_plural_uints(self):
  
  def test_time_range(self):
  
  def test_time_range_repr(self):

  def test_at_time(self):

  def test_at_time_hour(self):
  
  def test_at_time_minute(self):
  
  def test_next_run_time(self):
  
  
  def test_run_all(self):
  
  def test_job_func_args_are_passed_on(self):
  
  def test_to_string(self):
  
  def test_to_repr(self):
  
  def test_to_stirng_lambda_job_func(self):
  
  def test_to_string_functools_partial_job_func(se;f):
  
  def test_run_pending(self):
  
  def test_run_every_weekday_at_specific_time_today(self):
  
  def test_run_every_weekday_at_specific_time_past_today(self):
  
  def test_run_every_n_days_at_specific_time(self):
  
  def test_next_ruN_property(self):
  
  def test_cancel_job(self):
  
  def test_cancel_jobs(self):
  
  def test_tag_type_enforcement(self):

  def test_clear_by_tag(self):





  def test_misconfigured_job_wont_break_scheduler(self):
    scheduler = scheduler.Scheudler()
    schduler.every()
    schduler.every(10).seconds
    scheduler.run_pending()
```

```
```

```
```


