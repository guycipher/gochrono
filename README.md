![chrono](https://user-images.githubusercontent.com/5354910/118358070-739adb00-b57d-11eb-989b-68baf83f9584.png)

[![Go Report Card](https://goreportcard.com/badge/github.com/procyon-projects/chrono)](https://goreportcard.com/report/github.com/procyon-projects/chrono)
[![Build Status](https://travis-ci.com/procyon-projects/chrono.svg?branch=main)](https://travis-ci.com/procyon-projects/chrono)
[![codecov](https://codecov.io/gh/procyon-projects/chrono/branch/main/graph/badge.svg?token=OREV0YI8VU)](https://codecov.io/gh/procyon-projects/chrono)

Note:

```
This is an updated version of Chrono to support end of month, next run time, and more.
```

## Tested

```
        crons = []CRON{
            {Name: "Every 8 Hours", CRON: "0 0 */8 * * *"},
            {Name: "Every 8 Hours on the 30th Minute", CRON: "0 30 */8 * * *"},
            {Name: "Every 8 Hours on the 45th Minute", CRON: "0 45 */8 * * *"},

            {Name: "Every 9 Hours", CRON: "0 0 */9 * * *"},
            {Name: "Every 9 Hours on the 30th Minute", CRON: "0 30 */9 * * *"},
            {Name: "Every 9 Hours on the 45th Minute", CRON: "0 45 */9 * * *"},

            {Name: "Every 10 Hours", CRON: "0 0 */10 * * *"},
            {Name: "Every 10 Hours on the 30th Minute", CRON: "0 30 */10 * * *"},
            {Name: "Every 10 Hours on the 45th Minute", CRON: "0 45 */10 * * *"},

            {Name: "Every 11 Hours", CRON: "0 0 */11 * * *"},
            {Name: "Every 11 Hours on the 30th Minute", CRON: "0 30 */11 * * *"},
            {Name: "Every 11 Hours on the 45th Minute", CRON: "0 45 */11 * * *"},

            {Name: "Every 12 Hours", CRON: "0 0 */12 * * *"},
            {Name: "Every 12 Hours on the 30th Minute", CRON: "0 30 */12 * * *"},
            {Name: "Every 12 Hours on the 45th Minute", CRON: "0 45 */12 * * *"},

            {Name: "Every 13 Hours", CRON: "0 0 */13 * * *"},
            {Name: "Every 13 Hours on the 30th Minute", CRON: "0 30 */13 * * *"},
            {Name: "Every 13 Hours on the 45th Minute", CRON: "0 45 */13 * * *"},

            {Name: "Every 14 Hours", CRON: "0 0 */14 * * *"},
            {Name: "Every 14 Hours on the 30th Minute", CRON: "0 30 */14 * * *"},
            {Name: "Every 14 Hours on the 45th Minute", CRON: "0 45 */14 * * *"},

            {Name: "Every 15 Hours", CRON: "0 0 */15 * * *"},
            {Name: "Every 15 Hours on the 30th Minute", CRON: "0 30 */15 * * *"},
            {Name: "Every 15 Hours on the 45th Minute", CRON: "0 45 */15 * * *"},

            {Name: "Every 16 Hours", CRON: "0 0 */16 * * *"},
            {Name: "Every 16 Hours on the 30th Minute", CRON: "0 30 */16 * * *"},
            {Name: "Every 16 Hours on the 45th Minute", CRON: "0 45 */16 * * *"},

            {Name: "Every 17 Hours", CRON: "0 0 */17 * * *"},
            {Name: "Every 17 Hours on the 30th Minute", CRON: "0 30 */17 * * *"},
            {Name: "Every 17 Hours on the 45th Minute", CRON: "0 45 */17 * * *"},

            {Name: "Every 18 Hours", CRON: "0 0 */18 * * *"},
            {Name: "Every 18 Hours on the 30th Minute", CRON: "0 30 */18 * * *"},
            {Name: "Every 18 Hours on the 45th Minute", CRON: "0 45 */18 * * *"},

            {Name: "Every 19 Hours", CRON: "0 0 */19 * * *"},
            {Name: "Every 19 Hours on the 30th Minute", CRON: "0 30 */19 * * *"},
            {Name: "Every 19 Hours on the 45th Minute", CRON: "0 45 */19 * * *"},

            {Name: "Every 20 Hours", CRON: "0 0 */20 * * *"},
            {Name: "Every 20 Hours on the 30th Minute", CRON: "0 30 */20 * * *"},
            {Name: "Every 20 Hours on the 45th Minute", CRON: "0 45 */20 * * *"},

            {Name: "Every 21 Hours", CRON: "0 0 */21 * * *"},
            {Name: "Every 21 Hours on the 30th Minute", CRON: "0 30 */21 * * *"},
            {Name: "Every 21 Hours on the 45th Minute", CRON: "0 45 */21 * * *"},

            {Name: "Every 22 Hours", CRON: "0 0 */22 * * *"},
            {Name: "Every 22 Hours on the 30th Minute", CRON: "0 30 */22 * * *"},
            {Name: "Every 22 Hours on the 45th Minute", CRON: "0 45 */22 * * *"},

            {Name: "Every 23 Hours", CRON: "0 0 */23 * * *"},
            {Name: "Every 23 Hours on the 30th Minute", CRON: "0 30 */23 * * *"},
            {Name: "Every 23 Hours on the 45th Minute", CRON: "0 45 */23 * * *"},

            {Name: "Every 24 Hours", CRON: "0 0 */24 * * *"},

            {Name: "Every Day at 00:00", CRON: "0 0 0 * * *"},
            {Name: "Every Day at 00:30", CRON: "0 30 0 * * *"},
            {Name: "Every Day at 00:45", CRON: "0 45 0 * * *"},
            {Name: "Every Day at 00:59", CRON: "0 59 0 * * *"},

            {Name: "Every Day at 01:00", CRON: "0 0 1 * * *"},
            {Name: "Every Day at 01:30", CRON: "0 30 1 * * *"},
            {Name: "Every Day at 01:45", CRON: "0 45 1 * * *"},
            {Name: "Every Day at 01:59", CRON: "0 59 1 * * *"},

            {Name: "Every Day at 02:00", CRON: "0 0 2 * * *"},
            {Name: "Every Day at 02:30", CRON: "0 30 2 * * *"},
            {Name: "Every Day at 02:45", CRON: "0 45 2 * * *"},
            {Name: "Every Day at 02:59", CRON: "0 59 2 * * *"},

            {Name: "Every Day at 03:00", CRON: "0 0 3 * * *"},
            {Name: "Every Day at 03:30", CRON: "0 30 3 * * *"},
            {Name: "Every Day at 03:45", CRON: "0 45 3 * * *"},
            {Name: "Every Day at 03:59", CRON: "0 59 3 * * *"},

            {Name: "Every Day at 04:00", CRON: "0 0 4 * * *"},
            {Name: "Every Day at 04:30", CRON: "0 30 4 * * *"},
            {Name: "Every Day at 04:45", CRON: "0 45 4 * * *"},
            {Name: "Every Day at 04:59", CRON: "0 59 4 * * *"},

            {Name: "Every Day at 05:00", CRON: "0 0 5 * * *"},
            {Name: "Every Day at 05:30", CRON: "0 30 5 * * *"},
            {Name: "Every Day at 05:45", CRON: "0 45 5 * * *"},
            {Name: "Every Day at 05:59", CRON: "0 59 5 * * *"},

            {Name: "Every Day at 06:00", CRON: "0 0 6 * * *"},
            {Name: "Every Day at 06:30", CRON: "0 30 6 * * *"},
            {Name: "Every Day at 06:45", CRON: "0 45 6 * * *"},
            {Name: "Every Day at 06:59", CRON: "0 59 6 * * *"},

            {Name: "Every Day at 07:00", CRON: "0 0 7 * * *"},
            {Name: "Every Day at 07:30", CRON: "0 30 7 * * *"},
            {Name: "Every Day at 07:45", CRON: "0 45 7 * * *"},
            {Name: "Every Day at 07:59", CRON: "0 59 7 * * *"},

            {Name: "Every Day at 08:00", CRON: "0 0 8 * * *"},
            {Name: "Every Day at 08:30", CRON: "0 30 8 * * *"},
            {Name: "Every Day at 08:45", CRON: "0 45 8 * * *"},
            {Name: "Every Day at 08:59", CRON: "0 59 8 * * *"},

            {Name: "Every Day at 09:00", CRON: "0 0 9 * * *"},
            {Name: "Every Day at 09:30", CRON: "0 30 9 * * *"},
            {Name: "Every Day at 09:45", CRON: "0 45 9 * * *"},
            {Name: "Every Day at 09:59", CRON: "0 59 9 * * *"},

            {Name: "Every Day at 10:00", CRON: "0 0 10 * * *"},
            {Name: "Every Day at 10:30", CRON: "0 30 10 * * *"},
            {Name: "Every Day at 10:45", CRON: "0 45 10 * * *"},
            {Name: "Every Day at 10:59", CRON: "0 59 10 * * *"},

            {Name: "Every Day at 11:00", CRON: "0 0 11 * * *"},
            {Name: "Every Day at 11:30", CRON: "0 30 11 * * *"},
            {Name: "Every Day at 11:45", CRON: "0 45 11 * * *"},
            {Name: "Every Day at 11:59", CRON: "0 59 11 * * *"},

            {Name: "Every Day at 12:00", CRON: "0 0 12 * * *"},
            {Name: "Every Day at 12:30", CRON: "0 30 12 * * *"},
            {Name: "Every Day at 12:45", CRON: "0 45 12 * * *"},
            {Name: "Every Day at 12:59", CRON: "0 59 12 * * *"},

            {Name: "Every Day at 13:00", CRON: "0 0 13 * * *"},
            {Name: "Every Day at 13:30", CRON: "0 30 13 * * *"},
            {Name: "Every Day at 13:45", CRON: "0 45 13 * * *"},
            {Name: "Every Day at 13:59", CRON: "0 59 13 * * *"},

            {Name: "Every Day at 14:00", CRON: "0 0 14 * * *"},
            {Name: "Every Day at 14:30", CRON: "0 30 14 * * *"},
            {Name: "Every Day at 14:45", CRON: "0 45 14 * * *"},
            {Name: "Every Day at 14:59", CRON: "0 59 14 * * *"},

            {Name: "Every Day at 15:00", CRON: "0 0 15 * * *"},
            {Name: "Every Day at 15:30", CRON: "0 30 15 * * *"},
            {Name: "Every Day at 15:45", CRON: "0 45 15 * * *"},
            {Name: "Every Day at 15:59", CRON: "0 59 15 * * *"},

            {Name: "Every Day at 16:00", CRON: "0 0 16 * * *"},
            {Name: "Every Day at 16:30", CRON: "0 30 16 * * *"},
            {Name: "Every Day at 16:45", CRON: "0 45 16 * * *"},
            {Name: "Every Day at 16:59", CRON: "0 59 16 * * *"},

            {Name: "Every Day at 17:00", CRON: "0 0 17 * * *"},
            {Name: "Every Day at 17:30", CRON: "0 30 17 * * *"},
            {Name: "Every Day at 17:45", CRON: "0 45 17 * * *"},
            {Name: "Every Day at 17:59", CRON: "0 59 17 * * *"},

            {Name: "Every Day at 18:00", CRON: "0 0 18 * * *"},
            {Name: "Every Day at 18:30", CRON: "0 30 18 * * *"},
            {Name: "Every Day at 18:45", CRON: "0 45 18 * * *"},
            {Name: "Every Day at 18:59", CRON: "0 59 18 * * *"},

            {Name: "Every Day at 19:00", CRON: "0 0 19 * * *"},
            {Name: "Every Day at 19:30", CRON: "0 30 19 * * *"},
            {Name: "Every Day at 19:45", CRON: "0 45 19 * * *"},
            {Name: "Every Day at 19:59", CRON: "0 59 19 * * *"},

            {Name: "Every Day at 20:00", CRON: "0 0 20 * * *"},
            {Name: "Every Day at 20:30", CRON: "0 30 20 * * *"},
            {Name: "Every Day at 20:45", CRON: "0 45 20 * * *"},
            {Name: "Every Day at 20:59", CRON: "0 59 20 * * *"},

            {Name: "Every Day at 21:00", CRON: "0 0 21 * * *"},
            {Name: "Every Day at 21:30", CRON: "0 30 21 * * *"},
            {Name: "Every Day at 21:45", CRON: "0 45 21 * * *"},
            {Name: "Every Day at 21:59", CRON: "0 59 21 * * *"},

            {Name: "Every Day at 22:00", CRON: "0 0 22 * * *"},
            {Name: "Every Day at 22:30", CRON: "0 30 22 * * *"},
            {Name: "Every Day at 22:45", CRON: "0 45 22 * * *"},
            {Name: "Every Day at 22:59", CRON: "0 59 22 * * *"},

            {Name: "Every Day at 23:00", CRON: "0 0 23 * * *"},
            {Name: "Every Day at 23:30", CRON: "0 30 23 * * *"},
            {Name: "Every Day at 23:45", CRON: "0 45 23 * * *"},
            {Name: "Every Day at 23:59", CRON: "0 59 23 * * *"},

            {Name: "Every Monday at 00:00", CRON: "0 0 0 * * MON"},
            {Name: "Every Monday at 00:30", CRON: "0 30 0 * * MON"},
            {Name: "Every Monday at 00:45", CRON: "0 45 0 * * MON"},
            {Name: "Every Monday at 00:59", CRON: "0 59 0 * * MON"},

            {Name: "Every Monday at 01:00", CRON: "0 0 1 * * MON"},
            {Name: "Every Monday at 01:30", CRON: "0 30 1 * * MON"},
            {Name: "Every Monday at 01:45", CRON: "0 45 1 * * MON"},
            {Name: "Every Monday at 01:59", CRON: "0 59 1 * * MON"},

            {Name: "Every Monday at 02:00", CRON: "0 0 2 * * MON"},
            {Name: "Every Monday at 02:30", CRON: "0 30 2 * * MON"},
            {Name: "Every Monday at 02:45", CRON: "0 45 2 * * MON"},
            {Name: "Every Monday at 02:59", CRON: "0 59 2 * * MON"},

            {Name: "Every Monday at 03:00", CRON: "0 0 3 * * MON"},
            {Name: "Every Monday at 03:30", CRON: "0 30 3 * * MON"},
            {Name: "Every Monday at 03:45", CRON: "0 45 3 * * MON"},
            {Name: "Every Monday at 03:59", CRON: "0 59 3 * * MON"},

            {Name: "Every Monday at 04:00", CRON: "0 0 4 * * MON"},
            {Name: "Every Monday at 04:30", CRON: "0 30 4 * * MON"},
            {Name: "Every Monday at 04:45", CRON: "0 45 4 * * MON"},
            {Name: "Every Monday at 04:59", CRON: "0 59 4 * * MON"},

            {Name: "Every Monday at 05:00", CRON: "0 0 5 * * MON"},
            {Name: "Every Monday at 05:30", CRON: "0 30 5 * * MON"},
            {Name: "Every Monday at 05:45", CRON: "0 45 5 * * MON"},
            {Name: "Every Monday at 05:59", CRON: "0 59 5 * * MON"},

            {Name: "Every Monday at 06:00", CRON: "0 0 6 * * MON"},
            {Name: "Every Monday at 06:30", CRON: "0 30 6 * * MON"},
            {Name: "Every Monday at 06:45", CRON: "0 45 6 * * MON"},
            {Name: "Every Monday at 06:59", CRON: "0 59 6 * * MON"},

            {Name: "Every Monday at 07:00", CRON: "0 0 7 * * MON"},
            {Name: "Every Monday at 07:30", CRON: "0 30 7 * * MON"},
            {Name: "Every Monday at 07:45", CRON: "0 45 7 * * MON"},
            {Name: "Every Monday at 07:59", CRON: "0 59 7 * * MON"},

            {Name: "Every Monday at 08:00", CRON: "0 0 8 * * MON"},
            {Name: "Every Monday at 08:30", CRON: "0 30 8 * * MON"},
            {Name: "Every Monday at 08:45", CRON: "0 45 8 * * MON"},
            {Name: "Every Monday at 08:59", CRON: "0 59 8 * * MON"},

            {Name: "Every Monday at 09:00", CRON: "0 0 9 * * MON"},
            {Name: "Every Monday at 09:30", CRON: "0 30 9 * * MON"},
            {Name: "Every Monday at 09:45", CRON: "0 45 9 * * MON"},
            {Name: "Every Monday at 09:59", CRON: "0 59 9 * * MON"},

            {Name: "Every Monday at 10:00", CRON: "0 0 10 * * MON"},
            {Name: "Every Monday at 10:30", CRON: "0 30 10 * * MON"},
            {Name: "Every Monday at 10:45", CRON: "0 45 10 * * MON"},
            {Name: "Every Monday at 10:59", CRON: "0 59 10 * * MON"},

            {Name: "Every Monday at 11:00", CRON: "0 0 11 * * MON"},
            {Name: "Every Monday at 11:30", CRON: "0 30 11 * * MON"},
            {Name: "Every Monday at 11:45", CRON: "0 45 11 * * MON"},
            {Name: "Every Monday at 11:59", CRON: "0 59 11 * * MON"},

            {Name: "Every Monday at 12:00", CRON: "0 0 12 * * MON"},
            {Name: "Every Monday at 12:30", CRON: "0 30 12 * * MON"},
            {Name: "Every Monday at 12:45", CRON: "0 45 12 * * MON"},
            {Name: "Every Monday at 12:59", CRON: "0 59 12 * * MON"},

            {Name: "Every Monday at 13:00", CRON: "0 0 13 * * MON"},
            {Name: "Every Monday at 13:30", CRON: "0 30 13 * * MON"},
            {Name: "Every Monday at 13:45", CRON: "0 45 13 * * MON"},
            {Name: "Every Monday at 13:59", CRON: "0 59 13 * * MON"},

            {Name: "Every Monday at 14:00", CRON: "0 0 14 * * MON"},
            {Name: "Every Monday at 14:30", CRON: "0 30 14 * * MON"},
            {Name: "Every Monday at 14:45", CRON: "0 45 14 * * MON"},
            {Name: "Every Monday at 14:59", CRON: "0 59 14 * * MON"},

            {Name: "Every Monday at 15:00", CRON: "0 0 15 * * MON"},
            {Name: "Every Monday at 15:30", CRON: "0 30 15 * * MON"},
            {Name: "Every Monday at 15:45", CRON: "0 45 15 * * MON"},
            {Name: "Every Monday at 15:59", CRON: "0 59 15 * * MON"},

            {Name: "Every Monday at 16:00", CRON: "0 0 16 * * MON"},
            {Name: "Every Monday at 16:30", CRON: "0 30 16 * * MON"},
            {Name: "Every Monday at 16:20", CRON: "0 20 16 * * MON"},
            {Name: "Every Monday at 16:45", CRON: "0 45 16 * * MON"},
            {Name: "Every Monday at 16:59", CRON: "0 59 16 * * MON"},

            {Name: "Every Monday at 17:00", CRON: "0 0 17 * * MON"},
            {Name: "Every Monday at 17:30", CRON: "0 30 17 * * MON"},
            {Name: "Every Monday at 17:45", CRON: "0 45 17 * * MON"},
            {Name: "Every Monday at 17:59", CRON: "0 59 17 * * MON"},

            {Name: "Every Monday at 18:00", CRON: "0 0 18 * * MON"},
            {Name: "Every Monday at 18:30", CRON: "0 30 18 * * MON"},
            {Name: "Every Monday at 18:45", CRON: "0 45 18 * * MON"},
            {Name: "Every Monday at 18:59", CRON: "0 59 18 * * MON"},

            {Name: "Every Monday at 19:00", CRON: "0 0 19 * * MON"},
            {Name: "Every Monday at 19:30", CRON: "0 30 19 * * MON"},
            {Name: "Every Monday at 19:45", CRON: "0 45 19 * * MON"},
            {Name: "Every Monday at 19:59", CRON: "0 59 19 * * MON"},

            {Name: "Every Monday at 20:00", CRON: "0 0 20 * * MON"},
            {Name: "Every Monday at 20:30", CRON: "0 30 20 * * MON"},
            {Name: "Every Monday at 20:45", CRON: "0 45 20 * * MON"},
            {Name: "Every Monday at 20:59", CRON: "0 59 20 * * MON"},

            {Name: "Every Monday at 21:00", CRON: "0 0 21 * * MON"},
            {Name: "Every Monday at 21:30", CRON: "0 30 21 * * MON"},
            {Name: "Every Monday at 21:45", CRON: "0 45 21 * * MON"},
            {Name: "Every Monday at 21:59", CRON: "0 59 21 * * MON"},

            {Name: "Every Monday at 22:00", CRON: "0 0 22 * * MON"},
            {Name: "Every Monday at 22:30", CRON: "0 30 22 * * MON"},
            {Name: "Every Monday at 22:45", CRON: "0 45 22 * * MON"},
            {Name: "Every Monday at 22:59", CRON: "0 59 22 * * MON"},

            {Name: "Every Monday at 23:00", CRON: "0 0 23 * * MON"},
            {Name: "Every Monday at 23:30", CRON: "0 30 23 * * MON"},
            {Name: "Every Monday at 23:45", CRON: "0 45 23 * * MON"},
            {Name: "Every Monday at 23:59", CRON: "0 59 23 * * MON"},

            {Name: "Every Tuesday at 00:00", CRON: "0 0 0 * * TUE"},
            {Name: "Every Tuesday at 00:30", CRON: "0 30 0 * * TUE"},
            {Name: "Every Tuesday at 00:45", CRON: "0 45 0 * * TUE"},
            {Name: "Every Tuesday at 00:59", CRON: "0 59 0 * * TUE"},

            {Name: "Every Tuesday at 01:00", CRON: "0 0 1 * * TUE"},
            {Name: "Every Tuesday at 01:30", CRON: "0 30 1 * * TUE"},
            {Name: "Every Tuesday at 01:45", CRON: "0 45 1 * * TUE"},
            {Name: "Every Tuesday at 01:59", CRON: "0 59 1 * * TUE"},

            {Name: "Every Tuesday at 02:00", CRON: "0 0 2 * * TUE"},
            {Name: "Every Tuesday at 02:30", CRON: "0 30 2 * * TUE"},
            {Name: "Every Tuesday at 02:45", CRON: "0 45 2 * * TUE"},
            {Name: "Every Tuesday at 02:59", CRON: "0 59 2 * * TUE"},

            {Name: "Every Tuesday at 03:00", CRON: "0 0 3 * * TUE"},
            {Name: "Every Tuesday at 03:30", CRON: "0 30 3 * * TUE"},
            {Name: "Every Tuesday at 03:45", CRON: "0 45 3 * * TUE"},
            {Name: "Every Tuesday at 03:59", CRON: "0 59 3 * * TUE"},

            {Name: "Every Tuesday at 04:00", CRON: "0 0 4 * * TUE"},
            {Name: "Every Tuesday at 04:30", CRON: "0 30 4 * * TUE"},
            {Name: "Every Tuesday at 04:45", CRON: "0 45 4 * * TUE"},
            {Name: "Every Tuesday at 04:59", CRON: "0 59 4 * * TUE"},

            {Name: "Every Tuesday at 05:00", CRON: "0 0 5 * * TUE"},
            {Name: "Every Tuesday at 05:30", CRON: "0 30 5 * * TUE"},
            {Name: "Every Tuesday at 05:45", CRON: "0 45 5 * * TUE"},
            {Name: "Every Tuesday at 05:59", CRON: "0 59 5 * * TUE"},

            {Name: "Every Tuesday at 06:00", CRON: "0 0 6 * * TUE"},
            {Name: "Every Tuesday at 06:30", CRON: "0 30 6 * * TUE"},
            {Name: "Every Tuesday at 06:45", CRON: "0 45 6 * * TUE"},
            {Name: "Every Tuesday at 06:59", CRON: "0 59 6 * * TUE"},

            {Name: "Every Tuesday at 07:00", CRON: "0 0 7 * * TUE"},
            {Name: "Every Tuesday at 07:30", CRON: "0 30 7 * * TUE"},
            {Name: "Every Tuesday at 07:45", CRON: "0 45 7 * * TUE"},
            {Name: "Every Tuesday at 07:59", CRON: "0 59 7 * * TUE"},

            {Name: "Every Tuesday at 08:00", CRON: "0 0 8 * * TUE"},
            {Name: "Every Tuesday at 08:30", CRON: "0 30 8 * * TUE"},
            {Name: "Every Tuesday at 08:45", CRON: "0 45 8 * * TUE"},
            {Name: "Every Tuesday at 08:59", CRON: "0 59 8 * * TUE"},

            {Name: "Every Tuesday at 09:00", CRON: "0 0 9 * * TUE"},
            {Name: "Every Tuesday at 09:30", CRON: "0 30 9 * * TUE"},
            {Name: "Every Tuesday at 09:45", CRON: "0 45 9 * * TUE"},
            {Name: "Every Tuesday at 09:59", CRON: "0 59 9 * * TUE"},

            {Name: "Every Tuesday at 10:00", CRON: "0 0 10 * * TUE"},
            {Name: "Every Tuesday at 10:30", CRON: "0 30 10 * * TUE"},
            {Name: "Every Tuesday at 10:45", CRON: "0 45 10 * * TUE"},
            {Name: "Every Tuesday at 10:59", CRON: "0 59 10 * * TUE"},

            {Name: "Every Tuesday at 11:00", CRON: "0 0 11 * * TUE"},
            {Name: "Every Tuesday at 11:30", CRON: "0 30 11 * * TUE"},
            {Name: "Every Tuesday at 11:45", CRON: "0 45 11 * * TUE"},
            {Name: "Every Tuesday at 11:59", CRON: "0 59 11 * * TUE"},

            {Name: "Every Tuesday at 12:00", CRON: "0 0 12 * * TUE"},
            {Name: "Every Tuesday at 12:30", CRON: "0 30 12 * * TUE"},
            {Name: "Every Tuesday at 12:45", CRON: "0 45 12 * * TUE"},
            {Name: "Every Tuesday at 12:59", CRON: "0 59 12 * * TUE"},

            {Name: "Every Tuesday at 13:00", CRON: "0 0 13 * * TUE"},
            {Name: "Every Tuesday at 13:30", CRON: "0 30 13 * * TUE"},
            {Name: "Every Tuesday at 13:45", CRON: "0 45 13 * * TUE"},
            {Name: "Every Tuesday at 13:59", CRON: "0 59 13 * * TUE"},

            {Name: "Every Tuesday at 14:00", CRON: "0 0 14 * * TUE"},
            {Name: "Every Tuesday at 14:30", CRON: "0 30 14 * * TUE"},
            {Name: "Every Tuesday at 14:45", CRON: "0 45 14 * * TUE"},
            {Name: "Every Tuesday at 14:59", CRON: "0 59 14 * * TUE"},

            {Name: "Every Tuesday at 15:00", CRON: "0 0 15 * * TUE"},
            {Name: "Every Tuesday at 15:30", CRON: "0 30 15 * * TUE"},
            {Name: "Every Tuesday at 15:45", CRON: "0 45 15 * * TUE"},
            {Name: "Every Tuesday at 15:59", CRON: "0 59 15 * * TUE"},

            {Name: "Every Tuesday at 16:00", CRON: "0 0 16 * * TUE"},
            {Name: "Every Tuesday at 16:30", CRON: "0 30 16 * * TUE"},
            {Name: "Every Tuesday at 16:20", CRON: "0 20 16 * * TUE"},
            {Name: "Every Tuesday at 16:45", CRON: "0 45 16 * * TUE"},
            {Name: "Every Tuesday at 16:59", CRON: "0 59 16 * * TUE"},

            {Name: "Every Tuesday at 17:00", CRON: "0 0 17 * * TUE"},
            {Name: "Every Tuesday at 17:30", CRON: "0 30 17 * * TUE"},
            {Name: "Every Tuesday at 17:45", CRON: "0 45 17 * * TUE"},
            {Name: "Every Tuesday at 17:59", CRON: "0 59 17 * * TUE"},

            {Name: "Every Tuesday at 18:00", CRON: "0 0 18 * * TUE"},
            {Name: "Every Tuesday at 18:30", CRON: "0 30 18 * * TUE"},
            {Name: "Every Tuesday at 18:45", CRON: "0 45 18 * * TUE"},
            {Name: "Every Tuesday at 18:59", CRON: "0 59 18 * * TUE"},

            {Name: "Every Tuesday at 19:00", CRON: "0 0 19 * * TUE"},
            {Name: "Every Tuesday at 19:30", CRON: "0 30 19 * * TUE"},
            {Name: "Every Tuesday at 19:45", CRON: "0 45 19 * * TUE"},
            {Name: "Every Tuesday at 19:59", CRON: "0 59 19 * * TUE"},

            {Name: "Every Tuesday at 20:00", CRON: "0 0 20 * * TUE"},
            {Name: "Every Tuesday at 20:30", CRON: "0 30 20 * * TUE"},
            {Name: "Every Tuesday at 20:45", CRON: "0 45 20 * * TUE"},
            {Name: "Every Tuesday at 20:59", CRON: "0 59 20 * * TUE"},

            {Name: "Every Tuesday at 21:00", CRON: "0 0 21 * * TUE"},
            {Name: "Every Tuesday at 21:30", CRON: "0 30 21 * * TUE"},
            {Name: "Every Tuesday at 21:45", CRON: "0 45 21 * * TUE"},
            {Name: "Every Tuesday at 21:59", CRON: "0 59 21 * * TUE"},

            {Name: "Every Tuesday at 22:00", CRON: "0 0 22 * * TUE"},
            {Name: "Every Tuesday at 22:30", CRON: "0 30 22 * * TUE"},
            {Name: "Every Tuesday at 22:45", CRON: "0 45 22 * * TUE"},
            {Name: "Every Tuesday at 22:59", CRON: "0 59 22 * * TUE"},

            {Name: "Every Tuesday at 23:00", CRON: "0 0 23 * * TUE"},
            {Name: "Every Tuesday at 23:30", CRON: "0 30 23 * * TUE"},
            {Name: "Every Tuesday at 23:45", CRON: "0 45 23 * * TUE"},
            {Name: "Every Tuesday at 23:59", CRON: "0 59 23 * * TUE"},

            {Name: "Every Wednesday at 00:00", CRON: "0 0 0 * * WED"},
            {Name: "Every Wednesday at 00:30", CRON: "0 30 0 * * WED"},
            {Name: "Every Wednesday at 00:45", CRON: "0 45 0 * * WED"},
            {Name: "Every Wednesday at 00:59", CRON: "0 59 0 * * WED"},

            {Name: "Every Wednesday at 01:00", CRON: "0 0 1 * * WED"},
            {Name: "Every Wednesday at 01:30", CRON: "0 30 1 * * WED"},
            {Name: "Every Wednesday at 01:45", CRON: "0 45 1 * * WED"},
            {Name: "Every Wednesday at 01:59", CRON: "0 59 1 * * WED"},

            {Name: "Every Wednesday at 02:00", CRON: "0 0 2 * * WED"},
            {Name: "Every Wednesday at 02:30", CRON: "0 30 2 * * WED"},
            {Name: "Every Wednesday at 02:45", CRON: "0 45 2 * * WED"},
            {Name: "Every Wednesday at 02:59", CRON: "0 59 2 * * WED"},

            {Name: "Every Wednesday at 03:00", CRON: "0 0 3 * * WED"},
            {Name: "Every Wednesday at 03:30", CRON: "0 30 3 * * WED"},
            {Name: "Every Wednesday at 03:45", CRON: "0 45 3 * * WED"},
            {Name: "Every Wednesday at 03:59", CRON: "0 59 3 * * WED"},

            {Name: "Every Wednesday at 04:00", CRON: "0 0 4 * * WED"},
            {Name: "Every Wednesday at 04:30", CRON: "0 30 4 * * WED"},
            {Name: "Every Wednesday at 04:45", CRON: "0 45 4 * * WED"},
            {Name: "Every Wednesday at 04:59", CRON: "0 59 4 * * WED"},

            {Name: "Every Wednesday at 05:00", CRON: "0 0 5 * * WED"},
            {Name: "Every Wednesday at 05:30", CRON: "0 30 5 * * WED"},
            {Name: "Every Wednesday at 05:45", CRON: "0 45 5 * * WED"},
            {Name: "Every Wednesday at 05:59", CRON: "0 59 5 * * WED"},

            {Name: "Every Wednesday at 06:00", CRON: "0 0 6 * * WED"},
            {Name: "Every Wednesday at 06:30", CRON: "0 30 6 * * WED"},
            {Name: "Every Wednesday at 06:45", CRON: "0 45 6 * * WED"},
            {Name: "Every Wednesday at 06:59", CRON: "0 59 6 * * WED"},

            {Name: "Every Wednesday at 07:00", CRON: "0 0 7 * * WED"},
            {Name: "Every Wednesday at 07:30", CRON: "0 30 7 * * WED"},
            {Name: "Every Wednesday at 07:45", CRON: "0 45 7 * * WED"},
            {Name: "Every Wednesday at 07:59", CRON: "0 59 7 * * WED"},

            {Name: "Every Wednesday at 08:00", CRON: "0 0 8 * * WED"},
            {Name: "Every Wednesday at 08:30", CRON: "0 30 8 * * WED"},
            {Name: "Every Wednesday at 08:45", CRON: "0 45 8 * * WED"},
            {Name: "Every Wednesday at 08:59", CRON: "0 59 8 * * WED"},

            {Name: "Every Wednesday at 09:00", CRON: "0 0 9 * * WED"},
            {Name: "Every Wednesday at 09:30", CRON: "0 30 9 * * WED"},
            {Name: "Every Wednesday at 09:45", CRON: "0 45 9 * * WED"},
            {Name: "Every Wednesday at 09:59", CRON: "0 59 9 * * WED"},

            {Name: "Every Wednesday at 10:00", CRON: "0 0 10 * * WED"},
            {Name: "Every Wednesday at 10:30", CRON: "0 30 10 * * WED"},
            {Name: "Every Wednesday at 10:45", CRON: "0 45 10 * * WED"},
            {Name: "Every Wednesday at 10:59", CRON: "0 59 10 * * WED"},

            {Name: "Every Wednesday at 11:00", CRON: "0 0 11 * * WED"},
            {Name: "Every Wednesday at 11:30", CRON: "0 30 11 * * WED"},
            {Name: "Every Wednesday at 11:45", CRON: "0 45 11 * * WED"},
            {Name: "Every Wednesday at 11:59", CRON: "0 59 11 * * WED"},

            {Name: "Every Wednesday at 12:00", CRON: "0 0 12 * * WED"},
            {Name: "Every Wednesday at 12:30", CRON: "0 30 12 * * WED"},
            {Name: "Every Wednesday at 12:45", CRON: "0 45 12 * * WED"},
            {Name: "Every Wednesday at 12:59", CRON: "0 59 12 * * WED"},

            {Name: "Every Wednesday at 13:00", CRON: "0 0 13 * * WED"},
            {Name: "Every Wednesday at 13:30", CRON: "0 30 13 * * WED"},
            {Name: "Every Wednesday at 13:45", CRON: "0 45 13 * * WED"},
            {Name: "Every Wednesday at 13:59", CRON: "0 59 13 * * WED"},

            {Name: "Every Wednesday at 14:00", CRON: "0 0 14 * * WED"},
            {Name: "Every Wednesday at 14:30", CRON: "0 30 14 * * WED"},
            {Name: "Every Wednesday at 14:45", CRON: "0 45 14 * * WED"},
            {Name: "Every Wednesday at 14:59", CRON: "0 59 14 * * WED"},

            {Name: "Every Wednesday at 15:00", CRON: "0 0 15 * * WED"},
            {Name: "Every Wednesday at 15:30", CRON: "0 30 15 * * WED"},
            {Name: "Every Wednesday at 15:45", CRON: "0 45 15 * * WED"},
            {Name: "Every Wednesday at 15:59", CRON: "0 59 15 * * WED"},

            {Name: "Every Wednesday at 16:00", CRON: "0 0 16 * * WED"},
            {Name: "Every Wednesday at 16:30", CRON: "0 30 16 * * WED"},
            {Name: "Every Wednesday at 16:20", CRON: "0 20 16 * * WED"},
            {Name: "Every Wednesday at 16:45", CRON: "0 45 16 * * WED"},
            {Name: "Every Wednesday at 16:59", CRON: "0 59 16 * * WED"},

            {Name: "Every Wednesday at 17:00", CRON: "0 0 17 * * WED"},
            {Name: "Every Wednesday at 17:30", CRON: "0 30 17 * * WED"},
            {Name: "Every Wednesday at 17:45", CRON: "0 45 17 * * WED"},
            {Name: "Every Wednesday at 17:59", CRON: "0 59 17 * * WED"},

            {Name: "Every Wednesday at 18:00", CRON: "0 0 18 * * WED"},
            {Name: "Every Wednesday at 18:30", CRON: "0 30 18 * * WED"},
            {Name: "Every Wednesday at 18:45", CRON: "0 45 18 * * WED"},
            {Name: "Every Wednesday at 18:59", CRON: "0 59 18 * * WED"},

            {Name: "Every Wednesday at 19:00", CRON: "0 0 19 * * WED"},
            {Name: "Every Wednesday at 19:30", CRON: "0 30 19 * * WED"},
            {Name: "Every Wednesday at 19:45", CRON: "0 45 19 * * WED"},
            {Name: "Every Wednesday at 19:59", CRON: "0 59 19 * * WED"},

            {Name: "Every Wednesday at 20:00", CRON: "0 0 20 * * WED"},
            {Name: "Every Wednesday at 20:30", CRON: "0 30 20 * * WED"},
            {Name: "Every Wednesday at 20:45", CRON: "0 45 20 * * WED"},
            {Name: "Every Wednesday at 20:59", CRON: "0 59 20 * * WED"},

            {Name: "Every Wednesday at 21:00", CRON: "0 0 21 * * WED"},
            {Name: "Every Wednesday at 21:30", CRON: "0 30 21 * * WED"},
            {Name: "Every Wednesday at 21:45", CRON: "0 45 21 * * WED"},
            {Name: "Every Wednesday at 21:59", CRON: "0 59 21 * * WED"},

            {Name: "Every Wednesday at 22:00", CRON: "0 0 22 * * WED"},
            {Name: "Every Wednesday at 22:30", CRON: "0 30 22 * * WED"},
            {Name: "Every Wednesday at 22:45", CRON: "0 45 22 * * WED"},
            {Name: "Every Wednesday at 22:59", CRON: "0 59 22 * * WED"},

            {Name: "Every Wednesday at 23:00", CRON: "0 0 23 * * WED"},
            {Name: "Every Wednesday at 23:30", CRON: "0 30 23 * * WED"},
            {Name: "Every Wednesday at 23:45", CRON: "0 45 23 * * WED"},
            {Name: "Every Wednesday at 23:59", CRON: "0 59 23 * * WED"},

            {Name: "Every Thursday at 00:00", CRON: "0 0 0 * * THU"},
            {Name: "Every Thursday at 00:30", CRON: "0 30 0 * * THU"},
            {Name: "Every Thursday at 00:45", CRON: "0 45 0 * * THU"},
            {Name: "Every Thursday at 00:59", CRON: "0 59 0 * * THU"},

            {Name: "Every Thursday at 01:00", CRON: "0 0 1 * * THU"},
            {Name: "Every Thursday at 01:30", CRON: "0 30 1 * * THU"},
            {Name: "Every Thursday at 01:45", CRON: "0 45 1 * * THU"},
            {Name: "Every Thursday at 01:59", CRON: "0 59 1 * * THU"},

            {Name: "Every Thursday at 02:00", CRON: "0 0 2 * * THU"},
            {Name: "Every Thursday at 02:30", CRON: "0 30 2 * * THU"},
            {Name: "Every Thursday at 02:45", CRON: "0 45 2 * * THU"},
            {Name: "Every Thursday at 02:59", CRON: "0 59 2 * * THU"},

            {Name: "Every Thursday at 03:00", CRON: "0 0 3 * * THU"},
            {Name: "Every Thursday at 03:30", CRON: "0 30 3 * * THU"},
            {Name: "Every Thursday at 03:45", CRON: "0 45 3 * * THU"},
            {Name: "Every Thursday at 03:59", CRON: "0 59 3 * * THU"},

            {Name: "Every Thursday at 04:00", CRON: "0 0 4 * * THU"},
            {Name: "Every Thursday at 04:30", CRON: "0 30 4 * * THU"},
            {Name: "Every Thursday at 04:45", CRON: "0 45 4 * * THU"},
            {Name: "Every Thursday at 04:59", CRON: "0 59 4 * * THU"},

            {Name: "Every Thursday at 05:00", CRON: "0 0 5 * * THU"},
            {Name: "Every Thursday at 05:30", CRON: "0 30 5 * * THU"},
            {Name: "Every Thursday at 05:45", CRON: "0 45 5 * * THU"},
            {Name: "Every Thursday at 05:59", CRON: "0 59 5 * * THU"},

            {Name: "Every Thursday at 06:00", CRON: "0 0 6 * * THU"},
            {Name: "Every Thursday at 06:30", CRON: "0 30 6 * * THU"},
            {Name: "Every Thursday at 06:45", CRON: "0 45 6 * * THU"},
            {Name: "Every Thursday at 06:59", CRON: "0 59 6 * * THU"},

            {Name: "Every Thursday at 07:00", CRON: "0 0 7 * * THU"},
            {Name: "Every Thursday at 07:30", CRON: "0 30 7 * * THU"},
            {Name: "Every Thursday at 07:45", CRON: "0 45 7 * * THU"},
            {Name: "Every Thursday at 07:59", CRON: "0 59 7 * * THU"},

            {Name: "Every Thursday at 08:00", CRON: "0 0 8 * * THU"},
            {Name: "Every Thursday at 08:30", CRON: "0 30 8 * * THU"},
            {Name: "Every Thursday at 08:45", CRON: "0 45 8 * * THU"},
            {Name: "Every Thursday at 08:59", CRON: "0 59 8 * * THU"},

            {Name: "Every Thursday at 09:00", CRON: "0 0 9 * * THU"},
            {Name: "Every Thursday at 09:30", CRON: "0 30 9 * * THU"},
            {Name: "Every Thursday at 09:45", CRON: "0 45 9 * * THU"},
            {Name: "Every Thursday at 09:59", CRON: "0 59 9 * * THU"},

            {Name: "Every Thursday at 10:00", CRON: "0 0 10 * * THU"},
            {Name: "Every Thursday at 10:30", CRON: "0 30 10 * * THU"},
            {Name: "Every Thursday at 10:45", CRON: "0 45 10 * * THU"},
            {Name: "Every Thursday at 10:59", CRON: "0 59 10 * * THU"},

            {Name: "Every Thursday at 11:00", CRON: "0 0 11 * * THU"},
            {Name: "Every Thursday at 11:30", CRON: "0 30 11 * * THU"},
            {Name: "Every Thursday at 11:45", CRON: "0 45 11 * * THU"},
            {Name: "Every Thursday at 11:59", CRON: "0 59 11 * * THU"},

            {Name: "Every Thursday at 12:00", CRON: "0 0 12 * * THU"},
            {Name: "Every Thursday at 12:30", CRON: "0 30 12 * * THU"},
            {Name: "Every Thursday at 12:45", CRON: "0 45 12 * * THU"},
            {Name: "Every Thursday at 12:59", CRON: "0 59 12 * * THU"},

            {Name: "Every Thursday at 13:00", CRON: "0 0 13 * * THU"},
            {Name: "Every Thursday at 13:30", CRON: "0 30 13 * * THU"},
            {Name: "Every Thursday at 13:45", CRON: "0 45 13 * * THU"},
            {Name: "Every Thursday at 13:59", CRON: "0 59 13 * * THU"},

            {Name: "Every Thursday at 14:00", CRON: "0 0 14 * * THU"},
            {Name: "Every Thursday at 14:30", CRON: "0 30 14 * * THU"},
            {Name: "Every Thursday at 14:45", CRON: "0 45 14 * * THU"},
            {Name: "Every Thursday at 14:59", CRON: "0 59 14 * * THU"},

            {Name: "Every Thursday at 15:00", CRON: "0 0 15 * * THU"},
            {Name: "Every Thursday at 15:30", CRON: "0 30 15 * * THU"},
            {Name: "Every Thursday at 15:45", CRON: "0 45 15 * * THU"},
            {Name: "Every Thursday at 15:59", CRON: "0 59 15 * * THU"},

            {Name: "Every Thursday at 16:00", CRON: "0 0 16 * * THU"},
            {Name: "Every Thursday at 16:30", CRON: "0 30 16 * * THU"},
            {Name: "Every Thursday at 16:20", CRON: "0 20 16 * * THU"},
            {Name: "Every Thursday at 16:45", CRON: "0 45 16 * * THU"},
            {Name: "Every Thursday at 16:59", CRON: "0 59 16 * * THU"},

            {Name: "Every Thursday at 17:00", CRON: "0 0 17 * * THU"},
            {Name: "Every Thursday at 17:30", CRON: "0 30 17 * * THU"},
            {Name: "Every Thursday at 17:45", CRON: "0 45 17 * * THU"},
            {Name: "Every Thursday at 17:59", CRON: "0 59 17 * * THU"},

            {Name: "Every Thursday at 18:00", CRON: "0 0 18 * * THU"},
            {Name: "Every Thursday at 18:30", CRON: "0 30 18 * * THU"},
            {Name: "Every Thursday at 18:45", CRON: "0 45 18 * * THU"},
            {Name: "Every Thursday at 18:59", CRON: "0 59 18 * * THU"},

            {Name: "Every Thursday at 19:00", CRON: "0 0 19 * * THU"},
            {Name: "Every Thursday at 19:30", CRON: "0 30 19 * * THU"},
            {Name: "Every Thursday at 19:45", CRON: "0 45 19 * * THU"},
            {Name: "Every Thursday at 19:59", CRON: "0 59 19 * * THU"},

            {Name: "Every Thursday at 20:00", CRON: "0 0 20 * * THU"},
            {Name: "Every Thursday at 20:30", CRON: "0 30 20 * * THU"},
            {Name: "Every Thursday at 20:45", CRON: "0 45 20 * * THU"},
            {Name: "Every Thursday at 20:59", CRON: "0 59 20 * * THU"},

            {Name: "Every Thursday at 21:00", CRON: "0 0 21 * * THU"},
            {Name: "Every Thursday at 21:30", CRON: "0 30 21 * * THU"},
            {Name: "Every Thursday at 21:45", CRON: "0 45 21 * * THU"},
            {Name: "Every Thursday at 21:59", CRON: "0 59 21 * * THU"},

            {Name: "Every Thursday at 22:00", CRON: "0 0 22 * * THU"},
            {Name: "Every Thursday at 22:30", CRON: "0 30 22 * * THU"},
            {Name: "Every Thursday at 22:45", CRON: "0 45 22 * * THU"},
            {Name: "Every Thursday at 22:59", CRON: "0 59 22 * * THU"},

            {Name: "Every Thursday at 23:00", CRON: "0 0 23 * * THU"},
            {Name: "Every Thursday at 23:30", CRON: "0 30 23 * * THU"},
            {Name: "Every Thursday at 23:45", CRON: "0 45 23 * * THU"},
            {Name: "Every Thursday at 23:59", CRON: "0 59 23 * * THU"},

            {Name: "Every Friday at 00:00", CRON: "0 0 0 * * FRI"},
            {Name: "Every Friday at 00:30", CRON: "0 30 0 * * FRI"},
            {Name: "Every Friday at 00:45", CRON: "0 45 0 * * FRI"},
            {Name: "Every Friday at 00:59", CRON: "0 59 0 * * FRI"},

            {Name: "Every Friday at 01:00", CRON: "0 0 1 * * FRI"},
            {Name: "Every Friday at 01:30", CRON: "0 30 1 * * FRI"},
            {Name: "Every Friday at 01:45", CRON: "0 45 1 * * FRI"},
            {Name: "Every Friday at 01:59", CRON: "0 59 1 * * FRI"},

            {Name: "Every Friday at 02:00", CRON: "0 0 2 * * FRI"},
            {Name: "Every Friday at 02:30", CRON: "0 30 2 * * FRI"},
            {Name: "Every Friday at 02:45", CRON: "0 45 2 * * FRI"},
            {Name: "Every Friday at 02:59", CRON: "0 59 2 * * FRI"},

            {Name: "Every Friday at 03:00", CRON: "0 0 3 * * FRI"},
            {Name: "Every Friday at 03:30", CRON: "0 30 3 * * FRI"},
            {Name: "Every Friday at 03:45", CRON: "0 45 3 * * FRI"},
            {Name: "Every Friday at 03:59", CRON: "0 59 3 * * FRI"},

            {Name: "Every Friday at 04:00", CRON: "0 0 4 * * FRI"},
            {Name: "Every Friday at 04:30", CRON: "0 30 4 * * FRI"},
            {Name: "Every Friday at 04:45", CRON: "0 45 4 * * FRI"},
            {Name: "Every Friday at 04:59", CRON: "0 59 4 * * FRI"},

            {Name: "Every Friday at 05:00", CRON: "0 0 5 * * FRI"},
            {Name: "Every Friday at 05:30", CRON: "0 30 5 * * FRI"},
            {Name: "Every Friday at 05:45", CRON: "0 45 5 * * FRI"},
            {Name: "Every Friday at 05:59", CRON: "0 59 5 * * FRI"},

            {Name: "Every Friday at 06:00", CRON: "0 0 6 * * FRI"},
            {Name: "Every Friday at 06:30", CRON: "0 30 6 * * FRI"},
            {Name: "Every Friday at 06:45", CRON: "0 45 6 * * FRI"},
            {Name: "Every Friday at 06:59", CRON: "0 59 6 * * FRI"},

            {Name: "Every Friday at 07:00", CRON: "0 0 7 * * FRI"},
            {Name: "Every Friday at 07:30", CRON: "0 30 7 * * FRI"},
            {Name: "Every Friday at 07:45", CRON: "0 45 7 * * FRI"},
            {Name: "Every Friday at 07:59", CRON: "0 59 7 * * FRI"},

            {Name: "Every Friday at 08:00", CRON: "0 0 8 * * FRI"},
            {Name: "Every Friday at 08:30", CRON: "0 30 8 * * FRI"},
            {Name: "Every Friday at 08:45", CRON: "0 45 8 * * FRI"},
            {Name: "Every Friday at 08:59", CRON: "0 59 8 * * FRI"},

            {Name: "Every Friday at 09:00", CRON: "0 0 9 * * FRI"},
            {Name: "Every Friday at 09:30", CRON: "0 30 9 * * FRI"},
            {Name: "Every Friday at 09:45", CRON: "0 45 9 * * FRI"},
            {Name: "Every Friday at 09:59", CRON: "0 59 9 * * FRI"},

            {Name: "Every Friday at 10:00", CRON: "0 0 10 * * FRI"},
            {Name: "Every Friday at 10:30", CRON: "0 30 10 * * FRI"},
            {Name: "Every Friday at 10:45", CRON: "0 45 10 * * FRI"},
            {Name: "Every Friday at 10:59", CRON: "0 59 10 * * FRI"},

            {Name: "Every Friday at 11:00", CRON: "0 0 11 * * FRI"},
            {Name: "Every Friday at 11:30", CRON: "0 30 11 * * FRI"},
            {Name: "Every Friday at 11:45", CRON: "0 45 11 * * FRI"},
            {Name: "Every Friday at 11:59", CRON: "0 59 11 * * FRI"},

            {Name: "Every Friday at 12:00", CRON: "0 0 12 * * FRI"},
            {Name: "Every Friday at 12:30", CRON: "0 30 12 * * FRI"},
            {Name: "Every Friday at 12:45", CRON: "0 45 12 * * FRI"},
            {Name: "Every Friday at 12:59", CRON: "0 59 12 * * FRI"},

            {Name: "Every Friday at 13:00", CRON: "0 0 13 * * FRI"},
            {Name: "Every Friday at 13:30", CRON: "0 30 13 * * FRI"},
            {Name: "Every Friday at 13:45", CRON: "0 45 13 * * FRI"},
            {Name: "Every Friday at 13:59", CRON: "0 59 13 * * FRI"},

            {Name: "Every Friday at 14:00", CRON: "0 0 14 * * FRI"},
            {Name: "Every Friday at 14:30", CRON: "0 30 14 * * FRI"},
            {Name: "Every Friday at 14:45", CRON: "0 45 14 * * FRI"},
            {Name: "Every Friday at 14:59", CRON: "0 59 14 * * FRI"},

            {Name: "Every Friday at 15:00", CRON: "0 0 15 * * FRI"},
            {Name: "Every Friday at 15:30", CRON: "0 30 15 * * FRI"},
            {Name: "Every Friday at 15:45", CRON: "0 45 15 * * FRI"},
            {Name: "Every Friday at 15:59", CRON: "0 59 15 * * FRI"},

            {Name: "Every Friday at 16:00", CRON: "0 0 16 * * FRI"},
            {Name: "Every Friday at 16:30", CRON: "0 30 16 * * FRI"},
            {Name: "Every Friday at 16:20", CRON: "0 20 16 * * FRI"},
            {Name: "Every Friday at 16:45", CRON: "0 45 16 * * FRI"},
            {Name: "Every Friday at 16:59", CRON: "0 59 16 * * FRI"},

            {Name: "Every Friday at 17:00", CRON: "0 0 17 * * FRI"},
            {Name: "Every Friday at 17:30", CRON: "0 30 17 * * FRI"},
            {Name: "Every Friday at 17:45", CRON: "0 45 17 * * FRI"},
            {Name: "Every Friday at 17:59", CRON: "0 59 17 * * FRI"},

            {Name: "Every Friday at 18:00", CRON: "0 0 18 * * FRI"},
            {Name: "Every Friday at 18:30", CRON: "0 30 18 * * FRI"},
            {Name: "Every Friday at 18:45", CRON: "0 45 18 * * FRI"},
            {Name: "Every Friday at 18:59", CRON: "0 59 18 * * FRI"},

            {Name: "Every Friday at 19:00", CRON: "0 0 19 * * FRI"},
            {Name: "Every Friday at 19:30", CRON: "0 30 19 * * FRI"},
            {Name: "Every Friday at 19:45", CRON: "0 45 19 * * FRI"},
            {Name: "Every Friday at 19:59", CRON: "0 59 19 * * FRI"},

            {Name: "Every Friday at 20:00", CRON: "0 0 20 * * FRI"},
            {Name: "Every Friday at 20:30", CRON: "0 30 20 * * FRI"},
            {Name: "Every Friday at 20:45", CRON: "0 45 20 * * FRI"},
            {Name: "Every Friday at 20:59", CRON: "0 59 20 * * FRI"},

            {Name: "Every Friday at 21:00", CRON: "0 0 21 * * FRI"},
            {Name: "Every Friday at 21:30", CRON: "0 30 21 * * FRI"},
            {Name: "Every Friday at 21:45", CRON: "0 45 21 * * FRI"},
            {Name: "Every Friday at 21:59", CRON: "0 59 21 * * FRI"},

            {Name: "Every Friday at 22:00", CRON: "0 0 22 * * FRI"},
            {Name: "Every Friday at 22:30", CRON: "0 30 22 * * FRI"},
            {Name: "Every Friday at 22:45", CRON: "0 45 22 * * FRI"},
            {Name: "Every Friday at 22:59", CRON: "0 59 22 * * FRI"},

            {Name: "Every Friday at 23:00", CRON: "0 0 23 * * FRI"},
            {Name: "Every Friday at 23:30", CRON: "0 30 23 * * FRI"},
            {Name: "Every Friday at 23:45", CRON: "0 45 23 * * FRI"},
            {Name: "Every Friday at 23:59", CRON: "0 59 23 * * FRI"},

            {Name: "Every Saturday at 00:00", CRON: "0 0 0 * * SAT"},
            {Name: "Every Saturday at 00:30", CRON: "0 30 0 * * SAT"},
            {Name: "Every Saturday at 00:45", CRON: "0 45 0 * * SAT"},
            {Name: "Every Saturday at 00:59", CRON: "0 59 0 * * SAT"},

            {Name: "Every Saturday at 01:00", CRON: "0 0 1 * * SAT"},
            {Name: "Every Saturday at 01:30", CRON: "0 30 1 * * SAT"},
            {Name: "Every Saturday at 01:45", CRON: "0 45 1 * * SAT"},
            {Name: "Every Saturday at 01:59", CRON: "0 59 1 * * SAT"},

            {Name: "Every Saturday at 02:00", CRON: "0 0 2 * * SAT"},
            {Name: "Every Saturday at 02:30", CRON: "0 30 2 * * SAT"},
            {Name: "Every Saturday at 02:45", CRON: "0 45 2 * * SAT"},
            {Name: "Every Saturday at 02:59", CRON: "0 59 2 * * SAT"},

            {Name: "Every Saturday at 03:00", CRON: "0 0 3 * * SAT"},
            {Name: "Every Saturday at 03:30", CRON: "0 30 3 * * SAT"},
            {Name: "Every Saturday at 03:45", CRON: "0 45 3 * * SAT"},
            {Name: "Every Saturday at 03:59", CRON: "0 59 3 * * SAT"},

            {Name: "Every Saturday at 04:00", CRON: "0 0 4 * * SAT"},
            {Name: "Every Saturday at 04:30", CRON: "0 30 4 * * SAT"},
            {Name: "Every Saturday at 04:45", CRON: "0 45 4 * * SAT"},
            {Name: "Every Saturday at 04:59", CRON: "0 59 4 * * SAT"},

            {Name: "Every Saturday at 05:00", CRON: "0 0 5 * * SAT"},
            {Name: "Every Saturday at 05:30", CRON: "0 30 5 * * SAT"},
            {Name: "Every Saturday at 05:45", CRON: "0 45 5 * * SAT"},
            {Name: "Every Saturday at 05:59", CRON: "0 59 5 * * SAT"},

            {Name: "Every Saturday at 06:00", CRON: "0 0 6 * * SAT"},
            {Name: "Every Saturday at 06:30", CRON: "0 30 6 * * SAT"},
            {Name: "Every Saturday at 06:45", CRON: "0 45 6 * * SAT"},
            {Name: "Every Saturday at 06:59", CRON: "0 59 6 * * SAT"},

            {Name: "Every Saturday at 07:00", CRON: "0 0 7 * * SAT"},
            {Name: "Every Saturday at 07:30", CRON: "0 30 7 * * SAT"},
            {Name: "Every Saturday at 07:45", CRON: "0 45 7 * * SAT"},
            {Name: "Every Saturday at 07:59", CRON: "0 59 7 * * SAT"},

            {Name: "Every Saturday at 08:00", CRON: "0 0 8 * * SAT"},
            {Name: "Every Saturday at 08:30", CRON: "0 30 8 * * SAT"},
            {Name: "Every Saturday at 08:45", CRON: "0 45 8 * * SAT"},
            {Name: "Every Saturday at 08:59", CRON: "0 59 8 * * SAT"},

            {Name: "Every Saturday at 09:00", CRON: "0 0 9 * * SAT"},
            {Name: "Every Saturday at 09:30", CRON: "0 30 9 * * SAT"},
            {Name: "Every Saturday at 09:45", CRON: "0 45 9 * * SAT"},
            {Name: "Every Saturday at 09:59", CRON: "0 59 9 * * SAT"},

            {Name: "Every Saturday at 10:00", CRON: "0 0 10 * * SAT"},
            {Name: "Every Saturday at 10:30", CRON: "0 30 10 * * SAT"},
            {Name: "Every Saturday at 10:45", CRON: "0 45 10 * * SAT"},
            {Name: "Every Saturday at 10:59", CRON: "0 59 10 * * SAT"},

            {Name: "Every Saturday at 11:00", CRON: "0 0 11 * * SAT"},
            {Name: "Every Saturday at 11:30", CRON: "0 30 11 * * SAT"},
            {Name: "Every Saturday at 11:45", CRON: "0 45 11 * * SAT"},
            {Name: "Every Saturday at 11:59", CRON: "0 59 11 * * SAT"},

            {Name: "Every Saturday at 12:00", CRON: "0 0 12 * * SAT"},
            {Name: "Every Saturday at 12:30", CRON: "0 30 12 * * SAT"},
            {Name: "Every Saturday at 12:45", CRON: "0 45 12 * * SAT"},
            {Name: "Every Saturday at 12:59", CRON: "0 59 12 * * SAT"},

            {Name: "Every Saturday at 13:00", CRON: "0 0 13 * * SAT"},
            {Name: "Every Saturday at 13:30", CRON: "0 30 13 * * SAT"},
            {Name: "Every Saturday at 13:45", CRON: "0 45 13 * * SAT"},
            {Name: "Every Saturday at 13:59", CRON: "0 59 13 * * SAT"},

            {Name: "Every Saturday at 14:00", CRON: "0 0 14 * * SAT"},
            {Name: "Every Saturday at 14:30", CRON: "0 30 14 * * SAT"},
            {Name: "Every Saturday at 14:45", CRON: "0 45 14 * * SAT"},
            {Name: "Every Saturday at 14:59", CRON: "0 59 14 * * SAT"},

            {Name: "Every Saturday at 15:00", CRON: "0 0 15 * * SAT"},
            {Name: "Every Saturday at 15:30", CRON: "0 30 15 * * SAT"},
            {Name: "Every Saturday at 15:45", CRON: "0 45 15 * * SAT"},
            {Name: "Every Saturday at 15:59", CRON: "0 59 15 * * SAT"},

            {Name: "Every Saturday at 16:00", CRON: "0 0 16 * * SAT"},
            {Name: "Every Saturday at 16:30", CRON: "0 30 16 * * SAT"},
            {Name: "Every Saturday at 16:20", CRON: "0 20 16 * * SAT"},
            {Name: "Every Saturday at 16:45", CRON: "0 45 16 * * SAT"},
            {Name: "Every Saturday at 16:59", CRON: "0 59 16 * * SAT"},

            {Name: "Every Saturday at 17:00", CRON: "0 0 17 * * SAT"},
            {Name: "Every Saturday at 17:30", CRON: "0 30 17 * * SAT"},
            {Name: "Every Saturday at 17:45", CRON: "0 45 17 * * SAT"},
            {Name: "Every Saturday at 17:59", CRON: "0 59 17 * * SAT"},

            {Name: "Every Saturday at 18:00", CRON: "0 0 18 * * SAT"},
            {Name: "Every Saturday at 18:30", CRON: "0 30 18 * * SAT"},
            {Name: "Every Saturday at 18:45", CRON: "0 45 18 * * SAT"},
            {Name: "Every Saturday at 18:59", CRON: "0 59 18 * * SAT"},

            {Name: "Every Saturday at 19:00", CRON: "0 0 19 * * SAT"},
            {Name: "Every Saturday at 19:30", CRON: "0 30 19 * * SAT"},
            {Name: "Every Saturday at 19:45", CRON: "0 45 19 * * SAT"},
            {Name: "Every Saturday at 19:59", CRON: "0 59 19 * * SAT"},

            {Name: "Every Saturday at 20:00", CRON: "0 0 20 * * SAT"},
            {Name: "Every Saturday at 20:30", CRON: "0 30 20 * * SAT"},
            {Name: "Every Saturday at 20:45", CRON: "0 45 20 * * SAT"},
            {Name: "Every Saturday at 20:59", CRON: "0 59 20 * * SAT"},

            {Name: "Every Saturday at 21:00", CRON: "0 0 21 * * SAT"},
            {Name: "Every Saturday at 21:30", CRON: "0 30 21 * * SAT"},
            {Name: "Every Saturday at 21:45", CRON: "0 45 21 * * SAT"},
            {Name: "Every Saturday at 21:59", CRON: "0 59 21 * * SAT"},

            {Name: "Every Saturday at 22:00", CRON: "0 0 22 * * SAT"},
            {Name: "Every Saturday at 22:30", CRON: "0 30 22 * * SAT"},
            {Name: "Every Saturday at 22:45", CRON: "0 45 22 * * SAT"},
            {Name: "Every Saturday at 22:59", CRON: "0 59 22 * * SAT"},

            {Name: "Every Saturday at 23:00", CRON: "0 0 23 * * SAT"},
            {Name: "Every Saturday at 23:30", CRON: "0 30 23 * * SAT"},
            {Name: "Every Saturday at 23:45", CRON: "0 45 23 * * SAT"},
            {Name: "Every Saturday at 23:59", CRON: "0 59 23 * * SAT"},

            {Name: "Every Sunday at 00:00", CRON: "0 0 0 * * SUN"},
            {Name: "Every Sunday at 00:30", CRON: "0 30 0 * * SUN"},
            {Name: "Every Sunday at 00:45", CRON: "0 45 0 * * SUN"},
            {Name: "Every Sunday at 00:59", CRON: "0 59 0 * * SUN"},

            {Name: "Every Sunday at 01:00", CRON: "0 0 1 * * SUN"},
            {Name: "Every Sunday at 01:30", CRON: "0 30 1 * * SUN"},
            {Name: "Every Sunday at 01:45", CRON: "0 45 1 * * SUN"},
            {Name: "Every Sunday at 01:59", CRON: "0 59 1 * * SUN"},

            {Name: "Every Sunday at 02:00", CRON: "0 0 2 * * SUN"},
            {Name: "Every Sunday at 02:30", CRON: "0 30 2 * * SUN"},
            {Name: "Every Sunday at 02:45", CRON: "0 45 2 * * SUN"},
            {Name: "Every Sunday at 02:59", CRON: "0 59 2 * * SUN"},

            {Name: "Every Sunday at 03:00", CRON: "0 0 3 * * SUN"},
            {Name: "Every Sunday at 03:30", CRON: "0 30 3 * * SUN"},
            {Name: "Every Sunday at 03:45", CRON: "0 45 3 * * SUN"},
            {Name: "Every Sunday at 03:59", CRON: "0 59 3 * * SUN"},

            {Name: "Every Sunday at 04:00", CRON: "0 0 4 * * SUN"},
            {Name: "Every Sunday at 04:30", CRON: "0 30 4 * * SUN"},
            {Name: "Every Sunday at 04:45", CRON: "0 45 4 * * SUN"},
            {Name: "Every Sunday at 04:59", CRON: "0 59 4 * * SUN"},

            {Name: "Every Sunday at 05:00", CRON: "0 0 5 * * SUN"},
            {Name: "Every Sunday at 05:30", CRON: "0 30 5 * * SUN"},
            {Name: "Every Sunday at 05:45", CRON: "0 45 5 * * SUN"},
            {Name: "Every Sunday at 05:59", CRON: "0 59 5 * * SUN"},

            {Name: "Every Sunday at 06:00", CRON: "0 0 6 * * SUN"},
            {Name: "Every Sunday at 06:30", CRON: "0 30 6 * * SUN"},
            {Name: "Every Sunday at 06:45", CRON: "0 45 6 * * SUN"},
            {Name: "Every Sunday at 06:59", CRON: "0 59 6 * * SUN"},

            {Name: "Every Sunday at 07:00", CRON: "0 0 7 * * SUN"},
            {Name: "Every Sunday at 07:30", CRON: "0 30 7 * * SUN"},
            {Name: "Every Sunday at 07:45", CRON: "0 45 7 * * SUN"},
            {Name: "Every Sunday at 07:59", CRON: "0 59 7 * * SUN"},

            {Name: "Every Sunday at 08:00", CRON: "0 0 8 * * SUN"},
            {Name: "Every Sunday at 08:30", CRON: "0 30 8 * * SUN"},
            {Name: "Every Sunday at 08:45", CRON: "0 45 8 * * SUN"},
            {Name: "Every Sunday at 08:59", CRON: "0 59 8 * * SUN"},

            {Name: "Every Sunday at 09:00", CRON: "0 0 9 * * SUN"},
            {Name: "Every Sunday at 09:30", CRON: "0 30 9 * * SUN"},
            {Name: "Every Sunday at 09:45", CRON: "0 45 9 * * SUN"},
            {Name: "Every Sunday at 09:59", CRON: "0 59 9 * * SUN"},

            {Name: "Every Sunday at 10:00", CRON: "0 0 10 * * SUN"},
            {Name: "Every Sunday at 10:30", CRON: "0 30 10 * * SUN"},
            {Name: "Every Sunday at 10:45", CRON: "0 45 10 * * SUN"},
            {Name: "Every Sunday at 10:59", CRON: "0 59 10 * * SUN"},

            {Name: "Every Sunday at 11:00", CRON: "0 0 11 * * SUN"},
            {Name: "Every Sunday at 11:30", CRON: "0 30 11 * * SUN"},
            {Name: "Every Sunday at 11:45", CRON: "0 45 11 * * SUN"},
            {Name: "Every Sunday at 11:59", CRON: "0 59 11 * * SUN"},

            {Name: "Every Sunday at 12:00", CRON: "0 0 12 * * SUN"},
            {Name: "Every Sunday at 12:30", CRON: "0 30 12 * * SUN"},
            {Name: "Every Sunday at 12:45", CRON: "0 45 12 * * SUN"},
            {Name: "Every Sunday at 12:59", CRON: "0 59 12 * * SUN"},

            {Name: "Every Sunday at 13:00", CRON: "0 0 13 * * SUN"},
            {Name: "Every Sunday at 13:30", CRON: "0 30 13 * * SUN"},
            {Name: "Every Sunday at 13:45", CRON: "0 45 13 * * SUN"},
            {Name: "Every Sunday at 13:59", CRON: "0 59 13 * * SUN"},

            {Name: "Every Sunday at 14:00", CRON: "0 0 14 * * SUN"},
            {Name: "Every Sunday at 14:30", CRON: "0 30 14 * * SUN"},
            {Name: "Every Sunday at 14:45", CRON: "0 45 14 * * SUN"},
            {Name: "Every Sunday at 14:59", CRON: "0 59 14 * * SUN"},

            {Name: "Every Sunday at 15:00", CRON: "0 0 15 * * SUN"},
            {Name: "Every Sunday at 15:30", CRON: "0 30 15 * * SUN"},
            {Name: "Every Sunday at 15:45", CRON: "0 45 15 * * SUN"},
            {Name: "Every Sunday at 15:59", CRON: "0 59 15 * * SUN"},

            {Name: "Every Sunday at 16:00", CRON: "0 0 16 * * SUN"},
            {Name: "Every Sunday at 16:30", CRON: "0 30 16 * * SUN"},
            {Name: "Every Sunday at 16:20", CRON: "0 20 16 * * SUN"},
            {Name: "Every Sunday at 16:45", CRON: "0 45 16 * * SUN"},
            {Name: "Every Sunday at 16:59", CRON: "0 59 16 * * SUN"},

            {Name: "Every Sunday at 17:00", CRON: "0 0 17 * * SUN"},
            {Name: "Every Sunday at 17:30", CRON: "0 30 17 * * SUN"},
            {Name: "Every Sunday at 17:45", CRON: "0 45 17 * * SUN"},
            {Name: "Every Sunday at 17:59", CRON: "0 59 17 * * SUN"},

            {Name: "Every Sunday at 18:00", CRON: "0 0 18 * * SUN"},
            {Name: "Every Sunday at 18:30", CRON: "0 30 18 * * SUN"},
            {Name: "Every Sunday at 18:45", CRON: "0 45 18 * * SUN"},
            {Name: "Every Sunday at 18:59", CRON: "0 59 18 * * SUN"},

            {Name: "Every Sunday at 19:00", CRON: "0 0 19 * * SUN"},
            {Name: "Every Sunday at 19:30", CRON: "0 30 19 * * SUN"},
            {Name: "Every Sunday at 19:45", CRON: "0 45 19 * * SUN"},
            {Name: "Every Sunday at 19:59", CRON: "0 59 19 * * SUN"},

            {Name: "Every Sunday at 20:00", CRON: "0 0 20 * * SUN"},
            {Name: "Every Sunday at 20:30", CRON: "0 30 20 * * SUN"},
            {Name: "Every Sunday at 20:45", CRON: "0 45 20 * * SUN"},
            {Name: "Every Sunday at 20:59", CRON: "0 59 20 * * SUN"},

            {Name: "Every Sunday at 21:00", CRON: "0 0 21 * * SUN"},
            {Name: "Every Sunday at 21:30", CRON: "0 30 21 * * SUN"},
            {Name: "Every Sunday at 21:45", CRON: "0 45 21 * * SUN"},
            {Name: "Every Sunday at 21:59", CRON: "0 59 21 * * SUN"},

            {Name: "Every Sunday at 22:00", CRON: "0 0 22 * * SUN"},
            {Name: "Every Sunday at 22:30", CRON: "0 30 22 * * SUN"},
            {Name: "Every Sunday at 22:45", CRON: "0 45 22 * * SUN"},
            {Name: "Every Sunday at 22:59", CRON: "0 59 22 * * SUN"},

            {Name: "Every Sunday at 23:00", CRON: "0 0 23 * * SUN"},
            {Name: "Every Sunday at 23:30", CRON: "0 30 23 * * SUN"},
            {Name: "Every Sunday at 23:45", CRON: "0 45 23 * * SUN"},
            {Name: "Every Sunday at 23:59", CRON: "0 59 23 * * SUN"},


            {Name: "Every 1st of the Month at 00:00", CRON: "0 0 0 1 * *"},
            {Name: "Every 1st of the Month at 00:30", CRON: "0 30 0 1 * *"},
            {Name: "Every 1st of the Month at 00:45", CRON: "0 45 0 1 * *"},
            {Name: "Every 1st of the Month at 00:59", CRON: "0 59 0 1 * *"},

            {Name: "Every 1st of the Month at 01:00", CRON: "0 0 1 1 * *"},
            {Name: "Every 1st of the Month at 01:30", CRON: "0 30 1 1 * *"},
            {Name: "Every 1st of the Month at 01:45", CRON: "0 45 1 1 * *"},
            {Name: "Every 1st of the Month at 01:59", CRON: "0 59 1 1 * *"},

            {Name: "Every 1st of the Month at 02:00", CRON: "0 0 2 1 * *"},
            {Name: "Every 1st of the Month at 02:30", CRON: "0 30 2 1 * *"},
            {Name: "Every 1st of the Month at 02:45", CRON: "0 45 2 1 * *"},
            {Name: "Every 1st of the Month at 02:59", CRON: "0 59 2 1 * *"},

            {Name: "Every 1st of the Month at 03:00", CRON: "0 0 3 1 * *"},
            {Name: "Every 1st of the Month at 03:30", CRON: "0 30 3 1 * *"},
            {Name: "Every 1st of the Month at 03:45", CRON: "0 45 3 1 * *"},
            {Name: "Every 1st of the Month at 03:59", CRON: "0 59 3 1 * *"},

            {Name: "Every 1st of the Month at 04:00", CRON: "0 0 4 1 * *"},
            {Name: "Every 1st of the Month at 04:30", CRON: "0 30 4 1 * *"},
            {Name: "Every 1st of the Month at 04:45", CRON: "0 45 4 1 * *"},
            {Name: "Every 1st of the Month at 04:59", CRON: "0 59 4 1 * *"},

            {Name: "Every 1st of the Month at 05:00", CRON: "0 0 5 1 * *"},
            {Name: "Every 1st of the Month at 05:30", CRON: "0 30 5 1 * *"},
            {Name: "Every 1st of the Month at 05:45", CRON: "0 45 5 1 * *"},
            {Name: "Every 1st of the Month at 05:59", CRON: "0 59 5 1 * *"},

            {Name: "Every 1st of the Month at 06:00", CRON: "0 0 6 1 * *"},
            {Name: "Every 1st of the Month at 06:30", CRON: "0 30 6 1 * *"},
            {Name: "Every 1st of the Month at 06:45", CRON: "0 45 6 1 * *"},
            {Name: "Every 1st of the Month at 06:59", CRON: "0 59 6 1 * *"},

            {Name: "Every 1st of the Month at 07:00", CRON: "0 0 7 1 * *"},
            {Name: "Every 1st of the Month at 07:30", CRON: "0 30 7 1 * *"},
            {Name: "Every 1st of the Month at 07:45", CRON: "0 45 7 1 * *"},
            {Name: "Every 1st of the Month at 07:59", CRON: "0 59 7 1 * *"},

            {Name: "Every 1st of the Month at 08:00", CRON: "0 0 8 1 * *"},
            {Name: "Every 1st of the Month at 08:30", CRON: "0 30 8 1 * *"},
            {Name: "Every 1st of the Month at 08:45", CRON: "0 45 8 1 * *"},
            {Name: "Every 1st of the Month at 08:59", CRON: "0 59 8 1 * *"},

            {Name: "Every 1st of the Month at 09:00", CRON: "0 0 9 1 * *"},
            {Name: "Every 1st of the Month at 09:30", CRON: "0 30 9 1 * *"},
            {Name: "Every 1st of the Month at 09:45", CRON: "0 45 9 1 * *"},
            {Name: "Every 1st of the Month at 09:59", CRON: "0 59 9 1 * *"},

            {Name: "Every 1st of the Month at 10:00", CRON: "0 0 10 1 * *"},
            {Name: "Every 1st of the Month at 10:30", CRON: "0 30 10 1 * *"},
            {Name: "Every 1st of the Month at 10:45", CRON: "0 45 10 1 * *"},
            {Name: "Every 1st of the Month at 10:59", CRON: "0 59 10 1 * *"},

            {Name: "Every 1st of the Month at 11:00", CRON: "0 0 11 1 * *"},
            {Name: "Every 1st of the Month at 11:30", CRON: "0 30 11 1 * *"},
            {Name: "Every 1st of the Month at 11:45", CRON: "0 45 11 1 * *"},
            {Name: "Every 1st of the Month at 11:59", CRON: "0 59 11 1 * *"},

            {Name: "Every 1st of the Month at 12:00", CRON: "0 0 12 1 * *"},
            {Name: "Every 1st of the Month at 12:30", CRON: "0 30 12 1 * *"},
            {Name: "Every 1st of the Month at 12:45", CRON: "0 45 12 1 * *"},
            {Name: "Every 1st of the Month at 12:59", CRON: "0 59 12 1 * *"},

            {Name: "Every 1st of the Month at 13:00", CRON: "0 0 13 1 * *"},
            {Name: "Every 1st of the Month at 13:30", CRON: "0 30 13 1 * *"},
            {Name: "Every 1st of the Month at 13:45", CRON: "0 45 13 1 * *"},
            {Name: "Every 1st of the Month at 13:59", CRON: "0 59 13 1 * *"},

            {Name: "Every 1st of the Month at 14:00", CRON: "0 0 14 1 * *"},
            {Name: "Every 1st of the Month at 14:30", CRON: "0 30 14 1 * *"},
            {Name: "Every 1st of the Month at 14:45", CRON: "0 45 14 1 * *"},
            {Name: "Every 1st of the Month at 14:59", CRON: "0 59 14 1 * *"},

            {Name: "Every 1st of the Month at 15:00", CRON: "0 0 15 1 * *"},
            {Name: "Every 1st of the Month at 15:30", CRON: "0 30 15 1 * *"},
            {Name: "Every 1st of the Month at 15:45", CRON: "0 45 15 1 * *"},
            {Name: "Every 1st of the Month at 15:59", CRON: "0 59 15 1 * *"},

            {Name: "Every 1st of the Month at 16:00", CRON: "0 0 16 1 * *"},
            {Name: "Every 1st of the Month at 16:20", CRON: "0 20 16 1 * *"},
            {Name: "Every 1st of the Month at 16:30", CRON: "0 30 16 1 * *"},
            {Name: "Every 1st of the Month at 16:45", CRON: "0 45 16 1 * *"},
            {Name: "Every 1st of the Month at 16:59", CRON: "0 59 16 1 * *"},

            {Name: "Every 1st of the Month at 17:00", CRON: "0 0 17 1 * *"},
            {Name: "Every 1st of the Month at 17:30", CRON: "0 30 17 1 * *"},
            {Name: "Every 1st of the Month at 17:45", CRON: "0 45 17 1 * *"},
            {Name: "Every 1st of the Month at 17:59", CRON: "0 59 17 1 * *"},

            {Name: "Every 1st of the Month at 18:00", CRON: "0 0 18 1 * *"},
            {Name: "Every 1st of the Month at 18:30", CRON: "0 30 18 1 * *"},
            {Name: "Every 1st of the Month at 18:45", CRON: "0 45 18 1 * *"},
            {Name: "Every 1st of the Month at 18:59", CRON: "0 59 18 1 * *"},


            {Name: "Every 1st of the Month at 19:00", CRON: "0 0 19 1 * *"},
            {Name: "Every 1st of the Month at 19:30", CRON: "0 30 19 1 * *"},
            {Name: "Every 1st of the Month at 19:45", CRON: "0 45 19 1 * *"},
            {Name: "Every 1st of the Month at 19:59", CRON: "0 59 19 1 * *"},

            {Name: "Every 1st of the Month at 20:00", CRON: "0 0 20 1 * *"},
            {Name: "Every 1st of the Month at 20:30", CRON: "0 30 20 1 * *"},
            {Name: "Every 1st of the Month at 20:45", CRON: "0 45 20 1 * *"},
            {Name: "Every 1st of the Month at 20:59", CRON: "0 59 20 1 * *"},

            {Name: "Every 1st of the Month at 21:00", CRON: "0 0 21 1 * *"},
            {Name: "Every 1st of the Month at 21:30", CRON: "0 30 21 1 * *"},
            {Name: "Every 1st of the Month at 21:45", CRON: "0 45 21 1 * *"},
            {Name: "Every 1st of the Month at 21:59", CRON: "0 59 21 1 * *"},

            {Name: "Every 1st of the Month at 22:00", CRON: "0 0 22 1 * *"},
            {Name: "Every 1st of the Month at 22:30", CRON: "0 30 22 1 * *"},
            {Name: "Every 1st of the Month at 22:45", CRON: "0 45 22 1 * *"},
            {Name: "Every 1st of the Month at 22:59", CRON: "0 59 22 1 * *"},

            {Name: "Every 1st of the Month at 23:00", CRON: "0 0 23 1 * *"},
            {Name: "Every 1st of the Month at 23:30", CRON: "0 30 23 1 * *"},
            {Name: "Every 1st of the Month at 23:45", CRON: "0 45 23 1 * *"},
            {Name: "Every 1st of the Month at 23:59", CRON: "0 59 23 1 * *"},



            {Name: "Every other Month on the 1st at 00:00", CRON: "0 0 0 1 */2 *"},
            {Name: "Every other Month on the 1st at 00:30", CRON: "0 30 0 1 */2 *"},
            {Name: "Every other Month on the 1st at 00:45", CRON: "0 45 0 1 */2 *"},
            {Name: "Every other Month on the 1st at 00:59", CRON: "0 59 0 1 */2 *"},

            {Name: "Every other Month on the 1st at 01:00", CRON: "0 0 1 1 */2 *"},
            {Name: "Every other Month on the 1st at 01:30", CRON: "0 30 1 1 */2 *"},
            {Name: "Every other Month on the 1st at 01:45", CRON: "0 45 1 1 */2 *"},
            {Name: "Every other Month on the 1st at 01:59", CRON: "0 59 1 1 */2 *"},

            {Name: "Every other Month on the 1st at 02:00", CRON: "0 0 2 1 */2 *"},
            {Name: "Every other Month on the 1st at 02:30", CRON: "0 30 2 1 */2 *"},
            {Name: "Every other Month on the 1st at 02:45", CRON: "0 45 2 1 */2 *"},
            {Name: "Every other Month on the 1st at 02:59", CRON: "0 59 2 1 */2 *"},

            {Name: "Every other Month on the 1st at 03:00", CRON: "0 0 3 1 */2 *"},
            {Name: "Every other Month on the 1st at 03:30", CRON: "0 30 3 1 */2 *"},
            {Name: "Every other Month on the 1st at 03:45", CRON: "0 45 3 1 */2 *"},
            {Name: "Every other Month on the 1st at 03:59", CRON: "0 59 3 1 */2 *"},

            {Name: "Every other Month on the 1st at 04:00", CRON: "0 0 4 1 */2 *"},
            {Name: "Every other Month on the 1st at 04:30", CRON: "0 30 4 1 */2 *"},
            {Name: "Every other Month on the 1st at 04:45", CRON: "0 45 4 1 */2 *"},
            {Name: "Every other Month on the 1st at 04:59", CRON: "0 59 4 1 */2 *"},

            {Name: "Every other Month on the 1st at 05:00", CRON: "0 0 5 1 */2 *"},
            {Name: "Every other Month on the 1st at 05:30", CRON: "0 30 5 1 */2 *"},
            {Name: "Every other Month on the 1st at 05:45", CRON: "0 45 5 1 */2 *"},
            {Name: "Every other Month on the 1st at 05:59", CRON: "0 59 5 1 */2 *"},

            {Name: "Every other Month on the 1st at 06:00", CRON: "0 0 6 1 */2 *"},
            {Name: "Every other Month on the 1st at 06:30", CRON: "0 30 6 1 */2 *"},
            {Name: "Every other Month on the 1st at 06:45", CRON: "0 45 6 1 */2 *"},
            {Name: "Every other Month on the 1st at 06:59", CRON: "0 59 6 1 */2 *"},

            {Name: "Every other Month on the 1st at 07:00", CRON: "0 0 7 1 */2 *"},
            {Name: "Every other Month on the 1st at 07:30", CRON: "0 30 7 1 */2 *"},
            {Name: "Every other Month on the 1st at 07:45", CRON: "0 45 7 1 */2 *"},
            {Name: "Every other Month on the 1st at 07:59", CRON: "0 59 7 1 */2 *"},

            {Name: "Every other Month on the 1st at 08:00", CRON: "0 0 8 1 */2 *"},
            {Name: "Every other Month on the 1st at 08:30", CRON: "0 30 8 1 */2 *"},
            {Name: "Every other Month on the 1st at 08:45", CRON: "0 45 8 1 */2 *"},
            {Name: "Every other Month on the 1st at 08:59", CRON: "0 59 8 1 */2 *"},

            {Name: "Every other Month on the 1st at 09:00", CRON: "0 0 9 1 */2 *"},
            {Name: "Every other Month on the 1st at 09:30", CRON: "0 30 9 1 */2 *"},
            {Name: "Every other Month on the 1st at 09:45", CRON: "0 45 9 1 */2 *"},
            {Name: "Every other Month on the 1st at 09:59", CRON: "0 59 9 1 */2 *"},

            {Name: "Every other Month on the 1st at 10:00", CRON: "0 0 10 1 */2 *"},
            {Name: "Every other Month on the 1st at 10:30", CRON: "0 30 10 1 */2 *"},
            {Name: "Every other Month on the 1st at 10:45", CRON: "0 45 10 1 */2 *"},
            {Name: "Every other Month on the 1st at 10:59", CRON: "0 59 10 1 */2 *"},

            {Name: "Every other Month on the 1st at 11:00", CRON: "0 0 11 1 */2 *"},
            {Name: "Every other Month on the 1st at 11:30", CRON: "0 30 11 1 */2 *"},
            {Name: "Every other Month on the 1st at 11:45", CRON: "0 45 11 1 */2 *"},
            {Name: "Every other Month on the 1st at 11:59", CRON: "0 59 11 1 */2 *"},

            {Name: "Every other Month on the 1st at 12:00", CRON: "0 0 12 1 */2 *"},
            {Name: "Every other Month on the 1st at 12:30", CRON: "0 30 12 1 */2 *"},
            {Name: "Every other Month on the 1st at 12:45", CRON: "0 45 12 1 */2 *"},
            {Name: "Every other Month on the 1st at 12:59", CRON: "0 59 12 1 */2 *"},

            {Name: "Every other Month on the 1st at 13:00", CRON: "0 0 13 1 */2 *"},
            {Name: "Every other Month on the 1st at 13:30", CRON: "0 30 13 1 */2 *"},
            {Name: "Every other Month on the 1st at 13:45", CRON: "0 45 13 1 */2 *"},
            {Name: "Every other Month on the 1st at 13:59", CRON: "0 59 13 1 */2 *"},

            {Name: "Every other Month on the 1st at 14:00", CRON: "0 0 14 1 */2 *"},
            {Name: "Every other Month on the 1st at 14:30", CRON: "0 30 14 1 */2 *"},
            {Name: "Every other Month on the 1st at 14:45", CRON: "0 45 14 1 */2 *"},
            {Name: "Every other Month on the 1st at 14:59", CRON: "0 59 14 1 */2 *"},

            {Name: "Every other Month on the 1st at 15:00", CRON: "0 0 15 1 */2 *"},
            {Name: "Every other Month on the 1st at 15:30", CRON: "0 30 15 1 */2 *"},
            {Name: "Every other Month on the 1st at 15:45", CRON: "0 45 15 1 */2 *"},
            {Name: "Every other Month on the 1st at 15:59", CRON: "0 59 15 1 */2 *"},

            {Name: "Every other Month on the 1st at 16:00", CRON: "0 0 16 1 */2 *"},
            {Name: "Every other Month on the 1st at 16:20", CRON: "0 20 16 1 */2 *"},
            {Name: "Every other Month on the 1st at 16:30", CRON: "0 30 16 1 */2 *"},
            {Name: "Every other Month on the 1st at 16:45", CRON: "0 45 16 1 */2 *"},
            {Name: "Every other Month on the 1st at 16:59", CRON: "0 59 16 1 */2 *"},

            {Name: "Every other Month on the 1st at 17:00", CRON: "0 0 17 1 */2 *"},
            {Name: "Every other Month on the 1st at 17:30", CRON: "0 30 17 1 */2 *"},
            {Name: "Every other Month on the 1st at 17:45", CRON: "0 45 17 1 */2 *"},
            {Name: "Every other Month on the 1st at 17:59", CRON: "0 59 17 1 */2 *"},

            {Name: "Every other Month on the 1st at 18:00", CRON: "0 0 18 1 */2 *"},
            {Name: "Every other Month on the 1st at 18:30", CRON: "0 30 18 1 */2 *"},
            {Name: "Every other Month on the 1st at 18:45", CRON: "0 45 18 1 */2 *"},
            {Name: "Every other Month on the 1st at 18:59", CRON: "0 59 18 1 */2 *"},


            {Name: "Every other Month on the 1st at 19:00", CRON: "0 0 19 1 */2 *"},
            {Name: "Every other Month on the 1st at 19:30", CRON: "0 30 19 1 */2 *"},
            {Name: "Every other Month on the 1st at 19:45", CRON: "0 45 19 1 */2 *"},
            {Name: "Every other Month on the 1st at 19:59", CRON: "0 59 19 1 */2 *"},

            {Name: "Every other Month on the 1st at 20:00", CRON: "0 0 20 1 */2 *"},
            {Name: "Every other Month on the 1st at 20:30", CRON: "0 30 20 1 */2 *"},
            {Name: "Every other Month on the 1st at 20:45", CRON: "0 45 20 1 */2 *"},
            {Name: "Every other Month on the 1st at 20:59", CRON: "0 59 20 1 */2 *"},

            {Name: "Every other Month on the 1st at 21:00", CRON: "0 0 21 1 */2 *"},
            {Name: "Every other Month on the 1st at 21:30", CRON: "0 30 21 1 */2 *"},
            {Name: "Every other Month on the 1st at 21:45", CRON: "0 45 21 1 */2 *"},
            {Name: "Every other Month on the 1st at 21:59", CRON: "0 59 21 1 */2 *"},

            {Name: "Every other Month on the 1st at 22:00", CRON: "0 0 22 1 */2 *"},
            {Name: "Every other Month on the 1st at 22:30", CRON: "0 30 22 1 */2 *"},
            {Name: "Every other Month on the 1st at 22:45", CRON: "0 45 22 1 */2 *"},
            {Name: "Every other Month on the 1st at 22:59", CRON: "0 59 22 1 */2 *"},

            {Name: "Every other Month on the 1st at 23:00", CRON: "0 0 23 1 */2 *"},
            {Name: "Every other Month on the 1st at 23:30", CRON: "0 30 23 1 */2 *"},
            {Name: "Every other Month on the 1st at 23:45", CRON: "0 45 23 1 */2 *"},
            {Name: "Every other Month on the 1st at 23:59", CRON: "0 59 23 1 */2 *"},




            {Name: "Every 6 months on the 1st at 00:00", CRON: "0 0 0 1 */6 *"},
            {Name: "Every 6 months on the 1st at 00:30", CRON: "0 30 0 1 */6 *"},
            {Name: "Every 6 months on the 1st at 00:45", CRON: "0 45 0 1 */6 *"},
            {Name: "Every 6 months on the 1st at 00:59", CRON: "0 59 0 1 */6 *"},

            {Name: "Every 6 months on the 1st at 01:00", CRON: "0 0 1 1 */6 *"},
            {Name: "Every 6 months on the 1st at 01:30", CRON: "0 30 1 1 */6 *"},
            {Name: "Every 6 months on the 1st at 01:45", CRON: "0 45 1 1 */6 *"},
            {Name: "Every 6 months on the 1st at 01:59", CRON: "0 59 1 1 */6 *"},

            {Name: "Every 6 months on the 1st at 02:00", CRON: "0 0 2 1 */6 *"},
            {Name: "Every 6 months on the 1st at 02:30", CRON: "0 30 2 1 */6 *"},
            {Name: "Every 6 months on the 1st at 02:45", CRON: "0 45 2 1 */6 *"},
            {Name: "Every 6 months on the 1st at 02:59", CRON: "0 59 2 1 */6 *"},

            {Name: "Every 6 months on the 1st at 03:00", CRON: "0 0 3 1 */6 *"},
            {Name: "Every 6 months on the 1st at 03:30", CRON: "0 30 3 1 */6 *"},
            {Name: "Every 6 months on the 1st at 03:45", CRON: "0 45 3 1 */6 *"},
            {Name: "Every 6 months on the 1st at 03:59", CRON: "0 59 3 1 */6 *"},

            {Name: "Every 6 months on the 1st at 04:00", CRON: "0 0 4 1 */6 *"},
            {Name: "Every 6 months on the 1st at 04:30", CRON: "0 30 4 1 */6 *"},
            {Name: "Every 6 months on the 1st at 04:45", CRON: "0 45 4 1 */6 *"},
            {Name: "Every 6 months on the 1st at 04:59", CRON: "0 59 4 1 */6 *"},

            {Name: "Every 6 months on the 1st at 05:00", CRON: "0 0 5 1 */6 *"},
            {Name: "Every 6 months on the 1st at 05:30", CRON: "0 30 5 1 */6 *"},
            {Name: "Every 6 months on the 1st at 05:45", CRON: "0 45 5 1 */6 *"},
            {Name: "Every 6 months on the 1st at 05:59", CRON: "0 59 5 1 */6 *"},

            {Name: "Every 6 months on the 1st at 06:00", CRON: "0 0 6 1 */6 *"},
            {Name: "Every 6 months on the 1st at 06:30", CRON: "0 30 6 1 */6 *"},
            {Name: "Every 6 months on the 1st at 06:45", CRON: "0 45 6 1 */6 *"},
            {Name: "Every 6 months on the 1st at 06:59", CRON: "0 59 6 1 */6 *"},

            {Name: "Every 6 months on the 1st at 07:00", CRON: "0 0 7 1 */6 *"},
            {Name: "Every 6 months on the 1st at 07:30", CRON: "0 30 7 1 */6 *"},
            {Name: "Every 6 months on the 1st at 07:45", CRON: "0 45 7 1 */6 *"},
            {Name: "Every 6 months on the 1st at 07:59", CRON: "0 59 7 1 */6 *"},

            {Name: "Every 6 months on the 1st at 08:00", CRON: "0 0 8 1 */6 *"},
            {Name: "Every 6 months on the 1st at 08:30", CRON: "0 30 8 1 */6 *"},
            {Name: "Every 6 months on the 1st at 08:45", CRON: "0 45 8 1 */6 *"},
            {Name: "Every 6 months on the 1st at 08:59", CRON: "0 59 8 1 */6 *"},

            {Name: "Every 6 months on the 1st at 09:00", CRON: "0 0 9 1 */6 *"},
            {Name: "Every 6 months on the 1st at 09:30", CRON: "0 30 9 1 */6 *"},
            {Name: "Every 6 months on the 1st at 09:45", CRON: "0 45 9 1 */6 *"},
            {Name: "Every 6 months on the 1st at 09:59", CRON: "0 59 9 1 */6 *"},

            {Name: "Every 6 months on the 1st at 10:00", CRON: "0 0 10 1 */6 *"},
            {Name: "Every 6 months on the 1st at 10:30", CRON: "0 30 10 1 */6 *"},
            {Name: "Every 6 months on the 1st at 10:45", CRON: "0 45 10 1 */6 *"},
            {Name: "Every 6 months on the 1st at 10:59", CRON: "0 59 10 1 */6 *"},

            {Name: "Every 6 months on the 1st at 11:00", CRON: "0 0 11 1 */6 *"},
            {Name: "Every 6 months on the 1st at 11:30", CRON: "0 30 11 1 */6 *"},
            {Name: "Every 6 months on the 1st at 11:45", CRON: "0 45 11 1 */6 *"},
            {Name: "Every 6 months on the 1st at 11:59", CRON: "0 59 11 1 */6 *"},

            {Name: "Every 6 months on the 1st at 12:00", CRON: "0 0 12 1 */6 *"},
            {Name: "Every 6 months on the 1st at 12:30", CRON: "0 30 12 1 */6 *"},
            {Name: "Every 6 months on the 1st at 12:45", CRON: "0 45 12 1 */6 *"},
            {Name: "Every 6 months on the 1st at 12:59", CRON: "0 59 12 1 */6 *"},

            {Name: "Every 6 months on the 1st at 13:00", CRON: "0 0 13 1 */6 *"},
            {Name: "Every 6 months on the 1st at 13:30", CRON: "0 30 13 1 */6 *"},
            {Name: "Every 6 months on the 1st at 13:45", CRON: "0 45 13 1 */6 *"},
            {Name: "Every 6 months on the 1st at 13:59", CRON: "0 59 13 1 */6 *"},

            {Name: "Every 6 months on the 1st at 14:00", CRON: "0 0 14 1 */6 *"},
            {Name: "Every 6 months on the 1st at 14:30", CRON: "0 30 14 1 */6 *"},
            {Name: "Every 6 months on the 1st at 14:45", CRON: "0 45 14 1 */6 *"},
            {Name: "Every 6 months on the 1st at 14:59", CRON: "0 59 14 1 */6 *"},

            {Name: "Every 6 months on the 1st at 15:00", CRON: "0 0 15 1 */6 *"},
            {Name: "Every 6 months on the 1st at 15:30", CRON: "0 30 15 1 */6 *"},
            {Name: "Every 6 months on the 1st at 15:45", CRON: "0 45 15 1 */6 *"},
            {Name: "Every 6 months on the 1st at 15:59", CRON: "0 59 15 1 */6 *"},

            {Name: "Every 6 months on the 1st at 16:00", CRON: "0 0 16 1 */6 *"},
            {Name: "Every 6 months on the 1st at 16:20", CRON: "0 20 16 1 */6 *"},
            {Name: "Every 6 months on the 1st at 16:30", CRON: "0 30 16 1 */6 *"},
            {Name: "Every 6 months on the 1st at 16:45", CRON: "0 45 16 1 */6 *"},
            {Name: "Every 6 months on the 1st at 16:59", CRON: "0 59 16 1 */6 *"},

            {Name: "Every 6 months on the 1st at 17:00", CRON: "0 0 17 1 */6 *"},
            {Name: "Every 6 months on the 1st at 17:30", CRON: "0 30 17 1 */6 *"},
            {Name: "Every 6 months on the 1st at 17:45", CRON: "0 45 17 1 */6 *"},
            {Name: "Every 6 months on the 1st at 17:59", CRON: "0 59 17 1 */6 *"},

            {Name: "Every 6 months on the 1st at 18:00", CRON: "0 0 18 1 */6 *"},
            {Name: "Every 6 months on the 1st at 18:30", CRON: "0 30 18 1 */6 *"},
            {Name: "Every 6 months on the 1st at 18:45", CRON: "0 45 18 1 */6 *"},
            {Name: "Every 6 months on the 1st at 18:59", CRON: "0 59 18 1 */6 *"},


            {Name: "Every 6 months on the 1st at 19:00", CRON: "0 0 19 1 */6 *"},
            {Name: "Every 6 months on the 1st at 19:30", CRON: "0 30 19 1 */6 *"},
            {Name: "Every 6 months on the 1st at 19:45", CRON: "0 45 19 1 */6 *"},
            {Name: "Every 6 months on the 1st at 19:59", CRON: "0 59 19 1 */6 *"},

            {Name: "Every 6 months on the 1st at 20:00", CRON: "0 0 20 1 */6 *"},
            {Name: "Every 6 months on the 1st at 20:30", CRON: "0 30 20 1 */6 *"},
            {Name: "Every 6 months on the 1st at 20:45", CRON: "0 45 20 1 */6 *"},
            {Name: "Every 6 months on the 1st at 20:59", CRON: "0 59 20 1 */6 *"},

            {Name: "Every 6 months on the 1st at 21:00", CRON: "0 0 21 1 */6 *"},
            {Name: "Every 6 months on the 1st at 21:30", CRON: "0 30 21 1 */6 *"},
            {Name: "Every 6 months on the 1st at 21:45", CRON: "0 45 21 1 */6 *"},
            {Name: "Every 6 months on the 1st at 21:59", CRON: "0 59 21 1 */6 *"},

            {Name: "Every 6 months on the 1st at 22:00", CRON: "0 0 22 1 */6 *"},
            {Name: "Every 6 months on the 1st at 22:30", CRON: "0 30 22 1 */6 *"},
            {Name: "Every 6 months on the 1st at 22:45", CRON: "0 45 22 1 */6 *"},
            {Name: "Every 6 months on the 1st at 22:59", CRON: "0 59 22 1 */6 *"},

            {Name: "Every 6 months on the 1st at 23:00", CRON: "0 0 23 1 */6 *"},
            {Name: "Every 6 months on the 1st at 23:30", CRON: "0 30 23 1 */6 *"},
            {Name: "Every 6 months on the 1st at 23:45", CRON: "0 45 23 1 */6 *"},
            {Name: "Every 6 months on the 1st at 23:59", CRON: "0 59 23 1 */6 *"},


            {Name: "Every end of the month at 00:00", CRON: "0 0 0 L * ?"},
            {Name: "Every end of the month at 00:30", CRON: "0 30 0 L * ?"},
            {Name: "Every end of the month at 00:45", CRON: "0 45 0 L * ?"},
            {Name: "Every end of the month at 00:59", CRON: "0 59 0 L * ?"},

            {Name: "Every end of the month at 01:00", CRON: "0 0 1 L * ?"},
            {Name: "Every end of the month at 01:30", CRON: "0 30 1 L * ?"},
            {Name: "Every end of the month at 01:45", CRON: "0 45 1 L * ?"},
            {Name: "Every end of the month at 01:59", CRON: "0 59 1 L * ?"},

            {Name: "Every end of the month at 02:00", CRON: "0 0 2 L * ?"},
            {Name: "Every end of the month at 02:30", CRON: "0 30 2 L * ?"},
            {Name: "Every end of the month at 02:45", CRON: "0 45 2 L * ?"},
            {Name: "Every end of the month at 02:59", CRON: "0 59 2 L * ?"},

            {Name: "Every end of the month at 03:00", CRON: "0 0 3 L * ?"},
            {Name: "Every end of the month at 03:30", CRON: "0 30 3 L * ?"},
            {Name: "Every end of the month at 03:45", CRON: "0 45 3 L * ?"},
            {Name: "Every end of the month at 03:59", CRON: "0 59 3 L * ?"},

            {Name: "Every end of the month at 04:00", CRON: "0 0 4 L * ?"},
            {Name: "Every end of the month at 04:30", CRON: "0 30 4 L * ?"},
            {Name: "Every end of the month at 04:45", CRON: "0 45 4 L * ?"},
            {Name: "Every end of the month at 04:59", CRON: "0 59 4 L * ?"},

            {Name: "Every end of the month at 05:00", CRON: "0 0 5 L * ?"},
            {Name: "Every end of the month at 05:30", CRON: "0 30 5 L * ?"},
            {Name: "Every end of the month at 05:45", CRON: "0 45 5 L * ?"},
            {Name: "Every end of the month at 05:59", CRON: "0 59 5 L * ?"},

            {Name: "Every end of the month at 06:00", CRON: "0 0 6 L * ?"},
            {Name: "Every end of the month at 06:30", CRON: "0 30 6 L * ?"},
            {Name: "Every end of the month at 06:45", CRON: "0 45 6 L * ?"},
            {Name: "Every end of the month at 06:59", CRON: "0 59 6 L * ?"},

            {Name: "Every end of the month at 07:00", CRON: "0 0 7 L * ?"},
            {Name: "Every end of the month at 07:30", CRON: "0 30 7 L * ?"},
            {Name: "Every end of the month at 07:45", CRON: "0 45 7 L * ?"},
            {Name: "Every end of the month at 07:59", CRON: "0 59 7 L * ?"},

            {Name: "Every end of the month at 08:00", CRON: "0 0 8 L * ?"},
            {Name: "Every end of the month at 08:30", CRON: "0 30 8 L * ?"},
            {Name: "Every end of the month at 08:45", CRON: "0 45 8 L * ?"},
            {Name: "Every end of the month at 08:59", CRON: "0 59 8 L * ?"},

            {Name: "Every end of the month at 09:00", CRON: "0 0 9 L * ?"},
            {Name: "Every end of the month at 09:30", CRON: "0 30 9 L * ?"},
            {Name: "Every end of the month at 09:45", CRON: "0 45 9 L * ?"},
            {Name: "Every end of the month at 09:59", CRON: "0 59 9 L * ?"},

            {Name: "Every end of the month at 10:00", CRON: "0 0 10 L * ?"},
            {Name: "Every end of the month at 10:30", CRON: "0 30 10 L * ?"},
            {Name: "Every end of the month at 10:45", CRON: "0 45 10 L * ?"},
            {Name: "Every end of the month at 10:59", CRON: "0 59 10 L * ?"},

            {Name: "Every end of the month at 11:00", CRON: "0 0 11 L * ?"},
            {Name: "Every end of the month at 11:30", CRON: "0 30 11 L * ?"},
            {Name: "Every end of the month at 11:45", CRON: "0 45 11 L * ?"},
            {Name: "Every end of the month at 11:59", CRON: "0 59 11 L * ?"},

            {Name: "Every end of the month at 12:00", CRON: "0 0 12 L * ?"},
            {Name: "Every end of the month at 12:30", CRON: "0 30 12 L * ?"},
            {Name: "Every end of the month at 12:45", CRON: "0 45 12 L * ?"},
            {Name: "Every end of the month at 12:59", CRON: "0 59 12 L * ?"},

            {Name: "Every end of the month at 13:00", CRON: "0 0 13 L * ?"},
            {Name: "Every end of the month at 13:30", CRON: "0 30 13 L * ?"},
            {Name: "Every end of the month at 13:45", CRON: "0 45 13 L * ?"},
            {Name: "Every end of the month at 13:59", CRON: "0 59 13 L * ?"},

            {Name: "Every end of the month at 14:00", CRON: "0 0 14 L * ?"},
            {Name: "Every end of the month at 14:30", CRON: "0 30 14 L * ?"},
            {Name: "Every end of the month at 14:45", CRON: "0 45 14 L * ?"},
            {Name: "Every end of the month at 14:59", CRON: "0 59 14 L * ?"},

            {Name: "Every end of the month at 15:00", CRON: "0 0 15 L * ?"},
            {Name: "Every end of the month at 15:30", CRON: "0 30 15 L * ?"},
            {Name: "Every end of the month at 15:45", CRON: "0 45 15 L * ?"},
            {Name: "Every end of the month at 15:59", CRON: "0 59 15 L * ?"},

            {Name: "Every end of the month at 16:00", CRON: "0 0 16 L * ?"},
            {Name: "Every end of the month at 16:20", CRON: "0 20 16 L * ?"},
            {Name: "Every end of the month at 16:30", CRON: "0 30 16 L * ?"},
            {Name: "Every end of the month at 16:45", CRON: "0 45 16 L * ?"},
            {Name: "Every end of the month at 16:59", CRON: "0 59 16 L * ?"},

            {Name: "Every end of the month at 17:00", CRON: "0 0 17 L * ?"},
            {Name: "Every end of the month at 17:30", CRON: "0 30 17 L * ?"},
            {Name: "Every end of the month at 17:45", CRON: "0 45 17 L * ?"},
            {Name: "Every end of the month at 17:59", CRON: "0 59 17 L * ?"},

            {Name: "Every end of the month at 18:00", CRON: "0 0 18 L * ?"},
            {Name: "Every end of the month at 18:30", CRON: "0 30 18 L * ?"},
            {Name: "Every end of the month at 18:45", CRON: "0 45 18 L * ?"},
            {Name: "Every end of the month at 18:59", CRON: "0 59 18 L * ?"},

            {Name: "Every end of the month at 19:00", CRON: "0 0 19 L * ?"},
            {Name: "Every end of the month at 19:30", CRON: "0 30 19 L * ?"},
            {Name: "Every end of the month at 19:45", CRON: "0 45 19 L * ?"},
            {Name: "Every end of the month at 19:59", CRON: "0 59 19 L * ?"},

            {Name: "Every end of the month at 20:00", CRON: "0 0 20 L * ?"},
            {Name: "Every end of the month at 20:30", CRON: "0 30 20 L * ?"},
            {Name: "Every end of the month at 20:45", CRON: "0 45 20 L * ?"},
            {Name: "Every end of the month at 20:59", CRON: "0 59 20 L * ?"},

            {Name: "Every end of the month at 21:00", CRON: "0 0 21 L * ?"},
            {Name: "Every end of the month at 21:30", CRON: "0 30 21 L * ?"},
            {Name: "Every end of the month at 21:45", CRON: "0 45 21 L * ?"},
            {Name: "Every end of the month at 21:59", CRON: "0 59 21 L * ?"},

            {Name: "Every end of the month at 22:00", CRON: "0 0 22 L * ?"},
            {Name: "Every end of the month at 22:30", CRON: "0 30 22 L * ?"},
            {Name: "Every end of the month at 22:45", CRON: "0 45 22 L * ?"},
            {Name: "Every end of the month at 22:59", CRON: "0 59 22 L * ?"},

            {Name: "Every end of the month at 23:00", CRON: "0 0 23 L * ?"},
            {Name: "Every end of the month at 23:30", CRON: "0 30 23 L * ?"},
            {Name: "Every end of the month at 23:45", CRON: "0 45 23 L * ?"},
            {Name: "Every end of the month at 23:59", CRON: "0 59 23 L * ?"},




        }
```

Chrono is a scheduler library that lets you run your tasks and code periodically. It provides different scheduling functionalities to make it easier to create a scheduling task.

## Scheduling a One-Shot Task

The Schedule method helps us schedule the task to run once at the specified time. In the following example, the task will first be executed 1 second after the current time.
**WithTime** option is used to specify the execution time.

```go
taskScheduler := chrono.NewDefaultTaskScheduler()
now := time.Now()
startTime := now.Add(time.Second * 1)

task, err := taskScheduler.Schedule(func(ctx context.Context) {
	log.Print("One-Shot Task")
}, WithTime(startTime))

if err == nil {
	log.Print("Task has been scheduled successfully.")
}
```

Also, **WithStartTime** option can be used to specify the execution time. **But It's deprecated.**

```go
taskScheduler := chrono.NewDefaultTaskScheduler()

task, err := taskScheduler.Schedule(func(ctx context.Context) {
	log.Print("One-Shot Task")
}, WithStartTime(now.Year(), now.Month(), now.Day(), now.Hour(), now.Minute(), now.Second()+1))

if err == nil {
	log.Print("Task has been scheduled successfully.")
}
```

## Scheduling a Task with Fixed Delay

Let's schedule a task to run with a fixed delay between the finish time of the last execution of the task and the start time of the next execution of the task.
The fixed delay counts the delay after the completion of the last execution.

```go
taskScheduler := chrono.NewDefaultTaskScheduler()

task, err := taskScheduler.ScheduleWithFixedDelay(func(ctx context.Context) {
	log.Print("Fixed Delay Task")
	time.Sleep(3 * time.Second)
}, 5 * time.Second)

if err == nil {
	log.Print("Task has been scheduled successfully.")
}
```

Since the task itself takes 3 seconds to complete and we have specified a delay of 5 seconds between the finish time of the last execution of the task and the start time of the next execution of the task, there will be a delay of 8 seconds between each execution.

**WithStartTime** and **WithLocation** options can be combined with this.

## Schedule Task at a Fixed Rate

Let's schedule a task to run at a fixed rate of seconds.

```go
taskScheduler := chrono.NewDefaultTaskScheduler()

task, err := taskScheduler.ScheduleAtFixedRate(func(ctx context.Context) {
	log.Print("Fixed Rate of 5 seconds")
}, 5 * time.Second)

if err == nil {
	log.Print("Task has been scheduled successfully.")
}
```

The next task will run always after 5 seconds no matter the status of the previous task, which may be still running. So even if the previous task isn't done, the next task will run.
We can also use the **WithStartTime** option to specify the desired first execution time of the task.

```go
now := time.Now()

task, err := taskScheduler.ScheduleAtFixedRate(func(ctx context.Context) {
	log.Print("Fixed Rate of 5 seconds")
}, 5 * time.Second, WithStartTime(now.Year(), now.Month(), now.Day(), now.Hour(), now.Minute(), now.Second() + 2))
```

When we use this option, the task will run at the specified execution time and subsequently with the given period. In the above example, the task will first be executed 2 seconds after the current time.

We can also combine this option with **WithLocation** based on our requirements.

```go
now := time.Now()

task, err := taskScheduler.ScheduleAtFixedRate(func(ctx context.Context) {
	log.Print("Fixed Rate of 5 seconds")
}, 5 * time.Second, WithStartTime(now.Year(), now.Month(), now.Day(), 18, 45, 0),
WithLocation("America/New_York"))
```

In the above example, the task will first be executed at 18:45 of the current date in America/New York time.
**If the start time is in the past, the task will be executed immediately.**

## Scheduling a Task using Cron Expression

Sometimes Fixed Rate and Fixed Delay can not fulfill your needs, and we need the flexibility of cron expressions to schedule the execution of your tasks. With the help of the provided **ScheduleWithCron method**, we can schedule a task based on a cron expression.

```go
taskScheduler := chrono.NewDefaultTaskScheduler()

task, err := taskScheduler.ScheduleWithCron(func(ctx context.Context) {
	log.Print("Scheduled Task With Cron")
}, "0 45 18 10 * *")

if err == nil {
	log.Print("Task has been scheduled")
}
```

In this case, we're scheduling a task to be executed at 18:45 on the 10th day of every month

By default, the local time is used for the cron expression. However, we can use the **WithLocation** option to change this.

```go
task, err := taskScheduler.ScheduleWithCron(func(ctx context.Context) {
	log.Print("Scheduled Task With Cron")
}, "0 45 18 10 * *", WithLocation("America/New_York"))
```

In the above example, Task will be scheduled to be executed at 18:45 on the 10th day of every month in America/New York time.

**WithStartTimeoption** cannot be used with **ScheduleWithCron**.

## Canceling a Scheduled Task

Schedule methods return an instance of type ScheduledTask, which allows us to cancel a task or to check if the task is canceled. The Cancel method cancels the scheduled task but running tasks won't be interrupted.

```go
taskScheduler := chrono.NewDefaultTaskScheduler()

task, err := taskScheduler.ScheduleAtFixedRate(func(ctx context.Context) {
	log.Print("Fixed Rate of 5 seconds")
}, 5 * time.Second)

/* ... */

task.Cancel()
```

## Shutting Down a Scheduler

The **Shutdown()** method doesn't cause immediate shut down of the Scheduler and returns a channel. It will make the Scheduler stop accepting new tasks and shut down after all running tasks finish their current work.

```go
taskScheduler := chrono.NewDefaultTaskScheduler()

/* ... */

shutdownChannel := taskScheduler.Shutdown()
<- shutdownChannel

/* after all running task finished their works */
```

# License

Chrono is released under MIT License.
