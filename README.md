# Handmade Soap Store

A responsive e-commerce website for a handmade soap business. The platform presents the product range, provides product information, and enables customers to place orders through an agreed checkout or direct-order process.

## Project Objectives

- Establish a professional online presence for the soap brand.
- Showcase handmade products and product details.
- Help customers understand ingredients and product options.
- Provide a simple and reliable ordering experience.

## Key Features

- Homepage with brand introduction and featured products.
- Product catalogue and categories.
- Product detail pages with images, prices, ingredients, and descriptions.
- Shopping cart and agreed checkout or order-submission flow.
- Product bundles or gift sets, if offered.
- About the maker and brand story.
- Contact, FAQs, and delivery information.
- WhatsApp or phone ordering, where appropriate.

## Technology Stack

- **Frontend:** React.js, TypeScript
- **Backend:** Python, FastAPI
- **Database:** Supabase PostgreSQL
- **Authentication:** Supabase Auth, if customer accounts or protected management features are required
- **Storage:** Supabase Storage for product images, if required
- **Containerization:** Docker and Docker Compose

## Architecture

React provides the storefront and shopping interface. FastAPI handles custom business logic and order-related operations when needed. Supabase provides PostgreSQL database services and optional authentication or storage. Docker supports a consistent development environment.

## Getting Started

### Prerequisites

- Node.js and npm
- Python 3
- Docker and Docker Compose
- A Supabase project

### Environment Configuration

Create environment files based on `.env.example`.

Frontend variables:

- `VITE_SUPABASE_URL`
- `VITE_SUPABASE_ANON_KEY`

Backend variables, where needed:

- `SUPABASE_URL`
- `SUPABASE_SERVICE_ROLE_KEY` — server-side only, if elevated access is required.

Never commit production secrets or expose privileged credentials in the frontend.

### Development

Install frontend dependencies:

```bash
cd frontend
npm install
npm run dev
```

Configure the Python dependencies and FastAPI application entry point before starting the backend.

Once Docker configuration is complete, run:

```bash
docker compose up --build
```

## Initial Scope

The first release focuses on product discovery, product details, and a simple ordering flow. Online payment processing, recurring orders, advanced inventory management, and shipping integrations are excluded unless separately approved.

## Quality Assurance

Test product browsing, cart behavior, order submission, form validation, responsive layouts, and error handling.

## Project Status

In development.

## License

To be determined by the project owner.
