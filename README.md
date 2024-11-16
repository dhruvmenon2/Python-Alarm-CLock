import time

def alarm_clock():
    # Get the alarm time from the user
    alarm_time = input("Set the alarm time in HH:MM format (24-hour): ")

    print(f"Alarm set for {alarm_time}. Waiting...")

    while True:
        current_time = time.strftime("%H:%M")
        
        if current_time == alarm_time:
            print("Wake up! Alarm ringing!")
            break
      
        time.sleep(60)

if __name__ == "__main__":
    alarm_clock()
