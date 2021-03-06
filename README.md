CalendarBundle
==============

Provides applications with an events calendar. This bundle's model layer
represents a heavy port of Apple's iCal application.

*WARNING*: This is a prototype and not a final/stable bundle.

Features
--------

- Multiple Calendars
- Flexible Events
- Fully-implemented event recursion
- Event alarms
- Event RSVPs

Install
-------

Proceed with a normal bundle installation, and then execute the following steps:

Add to your config.yml:

    # app/config/config.yml
    rizza_calendar: ~

Add to your routing.yml:

    # app/config/routing.yml
    _calendar:
      resource: "@RizzaCalendar/Controller/CalendarController.php"
      type:     annotation

    _calendar_event:
    resource: "@RizzaCalendar/Controller/EventController.php"
    type:     annotation

TODO
----

- Create ODM models
- Commands
- Alternative storage backaends (Google Calendar, iCal feeds, etc.)
- Event hooks