# iwannabeyoursSAMU

import time
import os

# Color codes
RED = '\033[91m'
GREEN = '\033[91m'
BLUE = '\033[91m'
END_COLOR = '\033[0m'

def clear_screen():
    """Clear the screen"""
    os.system('cls' if os.name == 'nt' else 'clear')

def wait_until_timestamp(target_seconds):
    current_time = time.time()
    elapsed_time = current_time - start_time
    wait_time = target_seconds - elapsed_time
    if wait_time > 0:
        time.sleep(wait_time)

def print_lyrics():
    lyrics = [
        (17.45, "I wanna be your vacuum cleaner"),
        (22.24, "Breathing in your dust"),
        (24.90, "I wanna be your Ford Cortina"),
        (28.09, "I will never rust"),
        (31.82, "If you like your coffee hot"),
        (35.76, "Let me be your coffee pot"),
        (39.26, "You call the shots, babe"),
        (42.44, "I just wanna be yours"),
        (45.93, "Secrets I have held in my heart"),
        (49.38, "Are harder to hide than I thought"),
        (53.37, "Maybe I just wanna be yours"),
        (56.56, "I wanna be yours"),
        (58.68, "I wanna be yours"),
        (61.88, "Wanna be yours"),
        (65.61, "Wanna be yours"),
        (69.35, "Wanna be yours"),
        (75.18, "Let me be your 'leccy meter"),
        (78.15, "And I'll never run out"),
        (81.62, "Let me be the portable heater"),
        (84.59, "That you'll get cold without"),
        (87.56, "I wanna be your setting lotion"),
        (92.11, "Hold your hair in deep devotion (I'll be)"),
        (96.35, "At least as deep as the Pacific Ocean"),
        (99.04, "Now I wanna be yours"),
        (103.29, "Secrets I have held in my heart"),
        (106.76, "Are harder to hide than I thought"),
        (109.95, "Maybe I just wanna be yours"),
        (113.62, "I wanna be yours"),
        (115.27, "I wanna be yours"),
        (118.98, "Wanna be yours"),
        (122.71, "Wanna be yours"),
        (125.12, "Wanna be yours"),
        (129.37, "Wanna be yours"),
        (132.30, "Wanna be yours"),
        (135.49, "Wanna be yours"),
        (139.22, "Wanna be yours"),
        (141.33, "Wanna be yours"),
        (146.92, "I wanna be your vacuum cleaner (Wanna be yours)"),
        (150.08, "Breathing in your dust (Wanna be yours)"),
        (152.22, "I wanna be your Ford Cortina (Wanna be yours)"),
        (155.97, "I will never rust (Wanna be yours)"),
        (159.70, "I just wanna be yours (Wanna be yours)"),
        (163.15, "I just wanna be yours (Wanna be yours)"),
        (166.88, "I just wanna be yours (Wanna be yours)")
    ]

    print("I Wanna Be Yours - Arctic Monkeys")
    print("--------------------------------")
    print("SAMU")
    # time.sleep(1)

    global start_time
    start_time = time.time()

    for timestamp, text in lyrics:
        wait_until_timestamp(timestamp)
        
        # Clear screen
        clear_screen()
        
        # Split text into words and print word by word with color and love emoji
        words = text.split()
        current_line = ""
        
        for word in words:
            current_line += word + " "
            print(f"{BLUE}{current_line}{END_COLOR} ❤️")
            time.sleep(0.5)  # Adjust this delay as needed

if __name__ == "__main__":
    print_lyrics()
