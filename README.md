# api-blueprint
teste para documentação de api

Gerando documentação

npm install -g aglio

Para gerar a documentação podemos usar os comandos:

# Default theme
aglio -i input.apib -o output.html

# Use three-column layout
aglio -i input.apib --theme-template triple -o output.html

# Built-in color scheme
aglio --theme-variables slate -i input.apib -o output.html

# Customize a built-in style
aglio --theme-style default --theme-style ./my-style.less -i input.apib -o output.html

# Custom layout template
aglio --theme-template /path/to/template.jade -i input.apib -o output.html

# Custom theme engine
aglio -t my-engine -i input.apib -o output.html

# Run a live preview server on http://localhost:3000/
aglio -i input.apib -s

# Print output to terminal (useful for piping)
aglio -i input.apib -o -

# Disable condensing navigation links
aglio --no-theme-condense -i input.apib -o output.html

# Render full-width page instead of fixed max width
aglio --theme-full-width -i input.apib -o output.html

# Set an explicit file include path and read from stdin
aglio --include-path /path/to/includes -i - -o output.html

# Output verbose error information with stack traces
aglio -i input.apib -o output.html --verbose
