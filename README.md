# Open-me.py
def display_ascii_art():
    """
    Display a simple heart-shaped ASCII art.
    """
    heart_art = r"""
     *******       *******
   ***********   ***********
 ************* *************
*****************************
 ***************************
   ***********************
     *******************
       ***************
         ***********
           *******
             ***
              *
    """
    print(heart_art)

def display_text(text):
    """
    Display the provided text within a decorative border.
    """
    border = '*' * (len(text) + 4)
    print(border)
    print(f"* {text} *")
    print(border)

def main():
    
    display_ascii_art()

    while True:
        
        display_text("Can I be your valentine?")
        response = input("Your answer (Options: Yes, Definitely, Absolutely): ").strip().lower()

        
        if response in ['yes', 'definitely', 'absolutely']:
            display_text("Yay! I'm so happy!")
            break  
        elif response in ['ayoko', 'no']:
            display_text("Bawal ka tumanggi 😡😡😡")
          
        else:
            display_text("kulit sabing sa option lang mamimili e😡😡😡")
      

if __name__ == "__main__":
    main()
