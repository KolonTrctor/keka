import keyboard
import time
class HelloWold:
    def __init__(self):
       self.status = False
       keyboard.add_hotkey('g', self.start_stop)
    def start_stop(self):
        self.status = not self.status
    def run(self):
        while True:
            if self.status:
                time.sleep(1)
                keyboard.send("х")
                keyboard.send("у")
                keyboard.send("й")
                keyboard.send("Enter")
                print ("написал хуй")
                continue
            else:
                continue
helloworld = HelloWold()
helloworld.run()
