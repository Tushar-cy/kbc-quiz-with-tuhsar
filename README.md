# kbc-quiz-with-tuhsar
amitabh bachan fail , tumhara bhai hosting king lol
print("Deviyo aur Sajjanon, Swagat hai aap sabka KBC ke iss manch par! 🌟")
name = input("Enter your name: ")
print(f"Namaste {name}, chaliye shuru karte hain Kaun Banega Crorepati! 🎤\n")


kbc_questions = [
    ["Which planet is known as the 'Red Planet'?", "A) Venus", "B) Jupiter", "C) Mars", "D) Saturn"],
    ["Who wrote the Indian National Anthem?", "A) Rabindranath Tagore", "B) Bankim Chandra Chattopadhyay", "C) Mahatma Gandhi", "D) Subhas Chandra Bose"],
    ["What is the capital of Australia?", "A) Sydney", "B) Melbourne", "C) Canberra", "D) Perth"],
    ["Which Mughal emperor built the Taj Mahal?", "A) Akbar", "B) Jahangir", "C) Shah Jahan", "D) Aurangzeb"],
    ["Who is known as the 'Missile Man of India'?", "A) Vikram Sarabhai", "B) Abdul Kalam", "C) Rakesh Sharma", "D) C.V. Raman"],
    ["What is the SI unit of force?", "A) Watt", "B) Newton", "C) Pascal", "D) Joule"],
    ["Which river is known as the 'Sorrow of Bihar'?", "A) Yamuna", "B) Brahmaputra", "C) Kosi", "D) Ganga"],
    ["Which among these sports originated in India?", "A) Chess", "B) Table Tennis", "C) Golf", "D) Rugby"],
    ["What does CPU stand for in computing?", "A) Central Processing Unit", "B) Central Power Unit", "C) Central Performance Utility", "D) Central Programming Unit"],
    ["Which is the largest organ in the human body?", "A) Heart", "B) Brain", "C) Liver", "D) Skin"],
    ["In which year did India gain independence?", "A) 1945", "B) 1946", "C) 1947", "D) 1950"],
    ["Who discovered gravity?", "A) Albert Einstein", "B) Isaac Newton", "C) Galileo Galilei", "D) Nikola Tesla"],
    ["What is the national currency of Japan?", "A) Yuan", "B) Yen", "C) Ringgit", "D) Won"],
    ["Which element is necessary for respiration?", "A) Carbon Dioxide", "B) Hydrogen", "C) Oxygen", "D) Nitrogen"],
    ["Who was the first President of India?", "A) Sardar Patel", "B) Dr. Rajendra Prasad", "C) Jawaharlal Nehru", "D) B.R. Ambedkar"]
]


prizes = [
    "₹10,000", "₹20,000", "₹30,000", "₹50,000", "₹1,00,000",
    "₹1,60,000", "₹3,20,000", "₹6,40,000", "₹12,50,000", "₹25,00,000",
    "₹50,00,000", "₹1,00,00,000", "₹7,00,00,000", "Ambani mere L pe 🤣",
    "GOAT STATUS 🐐"
]


kbc_answers = [
    "C", "A", "C", "C", "B", "B", "C", "A", "A", "D", "C", "B", "B", "C", "B"
]

# Game Logic
i = 0
while i < 15:
    # Display question and options
    print(f"\nQuestion {i+1} for {prizes[i]}:")
    print(kbc_questions[i][0])  # Print the question
    for option in kbc_questions[i][1:]:  # Print options
        print(option)

     
    answer = input("Aapka jawab (A/B/C/D): ").strip().upper()

    
    if answer == kbc_answers[i]:
        print(f"✅ Sahi jawab! Aap jeet chuke hain {prizes[i]} 🏆")
    else:
        if i == 0:
            print("❌ Galat jawab! Aap kuch bhi nahi jeete. 😢 GAME OVER!")
        else:
            print(f"❌ Galat jawab! Aap jeete {prizes[i-1]} 🏆 GAME OVER!")
        break

    i += 1  # Move to the next question

    if i == 15:
        print("\n🎉 Yeah! Aapne JACKPOT jeet liya! 🤑🔥")

print("\nSamay barbaad ho gaya aapka, Ji Dhanyawad! 😂")
print("🚩 *RADHE RADHE* 🚩")
