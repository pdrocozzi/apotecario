# Apothecary: Ayurvedic Restaurant Web Application 🌿

A Ruby on Rails application that combines ancient Ayurvedic wisdom with modern plant-based nutrition.

## 🚀 Features

- **Dosha Quiz**: Interactive assessment to determine your Ayurvedic body type (Vata, Pitta, or Kapha)
- **Personalized Menu Recommendations**: Discover dishes tailored to your unique constitution
- **Nutritional Analysis**: Integration with nutrition APIs for detailed food information
- **User Profiles**: Save your preferences, dosha profile, and order history

## 💻 Tech Stack

- **Backend**: Ruby on Rails 7, PostgreSQL
- **Frontend**: Stimulus.js, TailwindCSS
- **Authentication**: Devise
- **API Integrations**: Nutrition APIs, OpenAI
- **Deployment**: Heroku

## 🛠️ Installation

```bash
# Clone the repository
git clone https://github.com/pdrocozzi/apotecario.git
cd apothecary

# Install dependencies
bundle install
yarn install

# Setup database
rails db:create
rails db:migrate
rails db:seed

# Start the server
bin/dev
```

## 🌱 Ayurvedic Principles

Apothecary is built on the foundation of Ayurvedic nutrition, which recognizes three main body types (doshas):

- **Vata**: Light, creative, quick-moving
- **Pitta**: Fiery, intelligent, ambitious
- **Kapha**: Earthy, stable, compassionate

Each dosha benefits from specific foods and cooking methods, which our application uses to make personalized recommendations.

## 📊 Database Schema

```
User
  - email
  - password
  - name

DoshaProfile
  - user_id
  - vata_score
  - pitta_score
  - kapha_score
  - primary_dosha
  - secondary_dosha

MenuItem
  - name
  - description
  - ingredients
  - price
  - vata_friendly
  - pitta_friendly
  - kapha_friendly
  - category

Recommendation
  - user_id
  - dosha_profile_id
  - recommendations
```

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check [issues page](https://github.com/pdrocozzi/apotecario/issues).

## 📝 License

This project is [MIT](LICENSE) licensed.

## 🙏 Acknowledgements

- Inspired by "Ayurveda & Nutrição Plant Based" by Marise Berg
- Built with love and respect for ancient wisdom
