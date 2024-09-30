

---
# High Level Context
## context
**Last Updated at:** 9/30/2024, 10:41:19 AM

Overview:
This Python module defines classes representing Zoom user and meeting data structures. It includes three main classes: User, Recordings, and Summary, which model the JSON structure of Zoom data.

User Class:
Represents a Zoom user with attributes like userid, firstname, lastname, email, and recordings.

Methods:
1. get_userid()
   Example: user.get_userid()

2. set_userid(userid)
   Example: user.set_userid("12345")

3. get_firstname()
   Example: user.get_firstname()

4. set_firstname(firstname)
   Example: user.set_firstname("John")

5. get_lastname()
   Example: user.get_lastname()

6. set_lastname(lastname)
   Example: user.set_lastname("Doe")

7. get_email()
   Example: user.get_email()

8. set_email(email)
   Example: user.set_email("john.doe@example.com")

9. get_recordings()
   Example: user.get_recordings()

10. set_recordings(recordings)
    Example: user.set_recordings([{"uuid": "abc123", "topic": "Meeting 1"}])

Recordings Class:
Represents a Zoom recording with attributes like uuid, topic, start_time, duration, vtt_content, and summary.

Methods:
1. get_uuid()
   Example: recording.get_uuid()

2. set_uuid(uuid)
   Example: recording.set_uuid("abc123")

3. get_topic()
   Example: recording.get_topic()

4. set_topic(topic)
   Example: recording.set_topic("Team Meeting")

5. get_start_time()
   Example: recording.get_start_time()

6. set_start_time(start_time)
   Example: recording.set_start_time("2023-06-15 14:00:00")

7. get_duration()
   Example: recording.get_duration()

8. set_duration(duration)
   Example: recording.set_duration("01:30:00")

9. get_vtt_content()
   Example: recording.get_vtt_content()

10. set_vtt_content(vtt_content)
    Example: recording.set_vtt_content("WEBVTT\n\n00:00:01.000 --> 00:00:05.000\nHello and welcome to the meeting.")

11. get_summary()
    Example: recording.get_summary()

12. set_summary(summary)
    Example: recording.set_summary({"summary_title": "Meeting Overview"})

Summary Class:
Represents a summary of a Zoom recording with attributes like summary_title, summary_overview, summary_details, and next_steps.

Methods:
1. get_summary_title()
   Example: summary.get_summary_title()

2. set_summary_title(summary_title)
   Example: summary.set_summary_title("Q2 Review Meeting")

3. get_summary_overview()
   Example: summary.get_summary_overview()

4. set_summary_overview(summary_overview)
   Example: summary.set_summary_overview("Discussed Q2 performance and goals for Q3.")

5. get_summary_details()
   Example: summary.get_summary_details()

6. set_summary_details(summary_details)
   Example: summary.set_summary_details(["Revenue increased by 15%", "Customer satisfaction improved"])

7. get_next_steps()
   Example: summary.get_next_steps()

8. set_next_steps(next_steps)
   Example: summary.set_next_steps(["Schedule follow-up meetings", "Prepare Q3 strategy document"])
