# Gravity Farms Petfood CMS Seed Repository

This repository contains a Contentstack seed configuration for a fictional pet food company called "Gravity Farms Petfood". It's designed to help you learn Contentstack CMS by providing a complete example with content types and sample entries.

## 🎯 Purpose

This seed repository demonstrates how to structure a Contentstack project with:
- **Content Types**: Homepage, Product, and Testimonial
- **Sample Entries**: Realistic data for a pet food website
- **References**: How to link content between different types

## 📁 Repository Structure

```
farm-fresh-pet-cms-seed/
├── content-types/
│   ├── homepage.json
│   ├── product.json
│   └── testimonial.json
├── entries/
│   ├── homepage/
│   │   └── homepage.json
│   ├── product/
│   │   ├── organic-chicken-kibble.json
│   │   └── salmon-snack-treats.json
│   └── testimonial/
│       ├── jane-doe.json
│       └── mike-smith.json
└── README.md
```

## 🏗️ Content Types

### Homepage
- **Hero Headline**: Main headline for the hero section
- **Hero Description**: Rich text description
- **Hero Image**: Background image for the hero section
- **Featured Products**: Reference field to showcase products
- **Call to Action**: Button text
- **SEO Fields**: Title and description for search optimization

### Product
- **Product Name**: Name of the pet food product
- **Description**: Rich text product description
- **Image**: Product photo
- **Price**: Product pricing
- **Category**: Dropdown (Dry Food, Wet Food, Treats, Supplements)
- **Pet Type**: Dropdown (Dog, Cat, Both)
- **Weight**: Product weight information
- **Ingredients**: Rich text ingredient list
- **SEO Fields**: Title and description

### Testimonial
- **Customer Name**: Name of the customer
- **Quote**: Rich text testimonial
- **Pet Name**: Name of the customer's pet
- **Pet Type**: Dropdown (Dog, Cat, Other)
- **Customer Photo**: Optional photo
- **Rating**: 1-5 star rating
- **Featured**: Boolean to highlight testimonials
- **Product Used**: Reference to the product they used

## 🚀 How to Use

### Prerequisites
1. Install the Contentstack CLI:
   ```bash
   npm install -g @contentstack/cli
   ```

2. Authenticate with Contentstack:
   ```bash
   npx @contentstack/cli --login
   ```

### Seeding Your Stack

1. **Clone this repository**:
   ```bash
   git clone https://github.com/your-username/farm-fresh-pet-cms-seed.git
   cd farm-fresh-pet-cms-seed
   ```

2. **Seed your Contentstack stack**:
   ```bash
   npx @contentstack/cli --stack:seed \
     --repo https://github.com/your-username/farm-fresh-pms-seed \
     --org <your-org-id> \
     --stack "Gravity Farms Petfood CMS"
   ```

   Replace:
   - `<your-org-id>` with your Contentstack organization ID
   - `your-username` with your GitHub username
   - Update the stack name as needed

### Alternative: Local Seeding

If you want to seed from your local directory:

```bash
npx @contentstack/cli --stack:seed \
  --path ./ \
  --org <your-org-id> \
  --stack "Gravity Farms Petfood CMS"
```

## 📝 What Happens After Seeding

After running the seed command, you'll have:

1. **Content Types**: Three content types (Homepage, Product, Testimonial) with all their fields
2. **Sample Entries**: 
   - 1 Homepage entry
   - 2 Product entries (Organic Chicken Kibble, Salmon Snack Treats)
   - 2 Testimonial entries (Jane Doe, Mike Smith)
3. **References**: Products linked to testimonials and featured on homepage

## 🎨 Next Steps

Once seeded, you can:

1. **Customize Content**: Edit the sample entries or create new ones
2. **Add More Content Types**: Extend the CMS with additional types like Blog, About Page, etc.
3. **Integrate with Frontend**: Use the Contentstack SDK to fetch and display content
4. **Set Up Webhooks**: Configure webhooks for real-time content updates
5. **Configure Workflows**: Set up content approval workflows

## 🔧 Customization

### Adding New Content Types
1. Create a new JSON file in `content-types/`
2. Follow the Contentstack schema format
3. Add sample entries in `entries/`

### Modifying Existing Types
1. Edit the JSON files in `content-types/`
2. Update corresponding entries in `entries/`
3. Re-seed or manually update your stack

## 📚 Learning Resources

- [Contentstack Documentation](https://www.contentstack.com/docs/)
- [Contentstack CLI Guide](https://www.contentstack.com/docs/developers/developer-hub/cli/)
- [Content Management API](https://www.contentstack.com/docs/developers/apis/content-management-api/)

## 🤝 Contributing

Feel free to fork this repository and customize it for your own projects. The structure is designed to be easily adaptable for different types of websites and applications.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Happy Contentstack Learning! 🐾** 