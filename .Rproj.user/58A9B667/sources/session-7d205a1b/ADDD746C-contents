library(shiny)

# UI
ui <- fluidPage(
  tags$head(
    tags$style(HTML("
      body {
        font-family: 'Lato', sans-serif;
        background-color: #f8f9fa;
      }

      .app-header {
        background: linear-gradient(to right, #3DB07C, #3DB07C);
        color: white;
        padding: 25px 40px;
        margin-bottom: 30px;
      }

      .app-header h2 {
        margin: 0;
        font-weight: 700;
      }

      .dataset-title {
        font-size: 22px;
        font-weight: 700;
        margin-top: 15px;
        margin-bottom: 5px;
      }

      .dataset-subtitle {
        font-size: 15px;
        color: #333;
        margin-bottom: 10px;
      }

      .dataset-card {
        background: white;
        border-radius: 10px;
        box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        overflow: hidden;
        margin: 0 auto 25px auto;
        max-width: 1100px;
        transition: transform 0.2s ease, box-shadow 0.2s ease;
      }

      .dataset-card:hover {
        transform: scale(1.01);
        box-shadow: 0 4px 12px rgba(0,0,0,0.2);
      }

      .dataset-header {
        padding: 20px;
        text-align: center;
      }

      .header-icon {
        font-size: 36px;
        color: white;
      }

      .info-row {
        display: flex;
        justify-content: space-between;
        align-items: center;
        font-weight: 600;
        margin-bottom: 15px;
        color: #555;
      }

      .info-left, .info-right {
        display: flex;
        align-items: center;
        font-size: 14px;
      }

      .info-left i, .info-right i {
        margin-right: 5px;
      }

      .view-btn {
        width: 100%;
        border-radius: 5px;
        padding: 10px;
        background-color: white;
        border: 2px solid #007bff;
        color: #007bff;
        font-weight: 600;
        text-align: center;
        text-decoration: none;
        display: inline-block;
      }

      .view-btn:hover {
        background-color: #007bff;
        color: white;
      }

      .footer {
        margin-top: 50px;
        text-align: center;
        color: gray;
        font-size: 13px;
      }
    "))
  ),
  
  div(class = "app-header",
      h2("Clinical RNA-seq Data Explorer"),
      span("Explore and analyze RNA sequencing datasets")
  ),
  
  h3(class = "text-center", "Available Datasets"),
  
  # Splice
  div(class = "dataset-card",
      div(class = "dataset-header", style = "background-color: #3DB07C;",
          icon("database", class = "header-icon")
      ),
      div(style = "padding: 20px;",
          div(class = "dataset-title", "Mrsd Splice"),
          div(class = "dataset-subtitle", "Contains RNA splicing data with gene and transcript information."),
          div(class = "info-row",
              div(class = "info-left", icon("table"), "5 columns"),
              div(class = "info-right", icon("list"), "6,747,459 rows")
          ),
          tags$a(
            href = "https://app.powerbi.com/view?r=eyJrIjoiNGZmMTMzMjItY2IwNC00MmJiLWI1OTctNTRkNTZhMWIwZmI5IiwidCI6ImE4M2RiYTUzLTEyNGQtNGQzMi04OGYwLWI3Mjg4OWE5ZTkyNiIsImMiOjN9",
            target = "_blank",
            class = "view-btn",
            icon("eye"), " View Dataset"
          )
      )
  ),
  
  # Vault
  div(class = "dataset-card",
      div(class = "dataset-header", style = "background-color: #3864D2;",
          icon("database", class = "header-icon")
      ),
      div(style = "padding: 20px;",
          div(class = "dataset-title", "Splice Vault"),
          div(class = "dataset-subtitle", "Contains detailed splice junction data with counts."),
          div(class = "info-row",
              div(class = "info-left", icon("table"), "20 columns"),
              div(class = "info-right", icon("list"), "6,747,459 rows")
          ),
          tags$a(
            href = "https://app.powerbi.com/view?r=eyJrIjoiNTZhZjIwN2UtOGM5Ni00NjAzLWExYzItYzc2NzdjYjM0YzdhIiwidCI6ImE4M2RiYTUzLTEyNGQtNGQzMi04OGYwLWI3Mjg4OWE5ZTkyNiIsImMiOjN9",
            target = "_blank",
            class = "view-btn",
            icon("eye"), " View Dataset"
          )
      )
  ),
  
  # Expression
  div(class = "dataset-card",
      div(class = "dataset-header", style = "background-color: #DE2D6D;",
          icon("database", class = "header-icon")
      ),
      div(style = "padding: 20px;",
          div(class = "dataset-title", "Mrsd Expression"),
          div(class = "dataset-subtitle", "Contains gene expression levels across different samples."),
          div(class = "info-row",
              div(class = "info-left", icon("table"), "15 columns"),
              div(class = "info-right", icon("list"), "7,654,321 rows")
          ),
          tags$a(
            href = "https://app.powerbi.com/view?r=eyJrIjoiNGZmMTMzMjItY2IwNC00MmJiLWI1OTctNTRkNTZhMWIwZmI5IiwidCI6ImE4M2RiYTUzLTEyNGQtNGQzMi04OGYwLWI3Mjg4OWE5ZTkyNiIsImMiOjN9",
            target = "_blank",
            class = "view-btn",
            icon("eye"), " View Dataset"
          )
      )
  ),
  
  div(class = "footer", "© 2025 RNA-seq Data Explorer")
)

server <- function(input, output, session) {}

shinyApp(ui, server)
