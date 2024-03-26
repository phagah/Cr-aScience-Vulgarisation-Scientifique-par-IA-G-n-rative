# Cr-aScience-Vulgarisation-Scientifique-par-IA-G-n-rative
CréaScience utilise l'IA générative et les modèles de langage avancés pour créer des contenus de vulgarisation scientifique attractifs et accessibles, adaptés aux différents niveaux de connaissances des lecteurs.
import random

# Placeholder for an advanced AI content generation model
def generate_content(topic, knowledge_level):
    # In a real application, this function would interface with an AI model to generate content.
    # Here, we simulate generated content with placeholders.
    if knowledge_level == 'beginner':
        return f"Introductory content on {topic}: Explaining basic concepts in an easy-to-understand manner."
    elif knowledge_level == 'intermediate':
        return f"Intermediate content on {topic}: Diving deeper into the subject with some technical details."
    else:  # Advanced
        return f"Advanced content on {topic}: Detailed exploration with technical and complex information."

def main():
    print("Welcome to CréaScience: Vulgarisation Scientifique par IA Générative!")
    topic = input("Please enter the scientific topic you're interested in: ")
    
    print("\nSelect your knowledge level:")
    print("1. Beginner")
    print("2. Intermediate")
    print("3. Advanced")
    knowledge_level_input = input("Enter the number corresponding to your level: ")
    
    knowledge_levels = {
        '1': 'beginner',
        '2': 'intermediate',
        '3': 'advanced'
    }
    
    knowledge_level = knowledge_levels.get(knowledge_level_input, 'beginner')
    
    generated_content = generate_content(topic, knowledge_level)
    print("\nGenerated Content:")
    print(generated_content)

if __name__ == "__main__":
    main()
