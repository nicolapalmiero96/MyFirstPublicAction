$GITHUB_OUTPUT è una variabile speciale di github

Vuol dire usa docker a partire da quell'immagine e passagli questi argomenti
  using: 'docker'
  image: 'Dockerfile'
  args:
    - ${{ inputs.who-to-greet }}


Checkout scarica il codice nella macchina virtuale
steps:
      - name: Checkout code
        uses: actions/checkout@v4.1.1