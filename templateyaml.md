# .github/workflows/deploy.yml
name: [What should we call this workflow?]

on:
  push:
    branches: [______]  # Which branch triggers deployment?
    paths: [______]     # Which file change should trigger it?

jobs:
  deploy:
    runs-on: ______     # What OS environment do we need?
    
    # Critical: What permissions does deploying to Pages require?
    permissions:
      contents: ______
      pages: ______
      id-token: ______
    
    steps:
      # Step 1: Get the code
      - name: ______
        uses: ______@______
      
      # Step 2: Configure GitHub Pages
      - name: ______
        uses: ______@______
        with:
          # What needs to be configured here?
      
      # Step 3: Upload the site as an artifact
      - name: ______
        uses: ______@______
        with:
          # What path contains our static files?
      
      # Step 4: Deploy to GitHub Pages
      - name: ______
        uses: ______@______
        with:
          # What artifact do we deploy?