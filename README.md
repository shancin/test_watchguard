# test_wachguard


   default Date getPeriodEnd(final Date periodStart, final Date minDate) {
      Date loopDate = periodStart;
      while (compareDates(loopDate, minDate) <0) {
         loopDate = getCalendarDay(getCurrentPeriodEnd(loopDate), 1);
      }
      return loopDate;
   }
