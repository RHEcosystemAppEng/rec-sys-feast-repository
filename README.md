# Recomendation System Feast repository
This repository implements a Feast feature store for a recommendation system, managing user, item, and interaction data with embeddings for user personalization.
## Usage
This feast-repository used by the rec-sys-gitops to deploy Rec-Sys Validated Patterns.

# TODO 
* add link for the rec-sys-gitops repo
* add link for the validated Patterns
* fix in `feature_store.py` the namespace and service name for online offline and repository.

## Features
- **User Features**: Age, gender, preferences.
- **Item Features**: Category, price, ratings, flags (popular, new_arrival, on_sale).
- **Interactions**: User-item interactions (view, cart, purchase, rate).
- **Embeddings**: Item and user embeddings with cosine similarity indexing; top-k item IDs per user.

## Setup

1. **Install dependencies**: `uv sync`
1. **Install dependencies**: `source .venv/bin/activate `
2. **Generate Data**: Run `python data_gen.py`
3. **Initialize Feast**: run `feast apply` from that directory.
