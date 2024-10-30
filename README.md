# presentationonR
Made a presentaion using R studio
install.packages("officer")
install.packages("magrittr")  # For piping (%>%)

# Load the necessary libraries
library(officer)
library(magrittr)

# Create a new PowerPoint presentation
ppt <- read_pptx()

# Add a title slide
ppt <- ppt %>%
  add_slide(layout = "Title Slide", master = "Office Theme") %>%
  ph_with_text(type = "ctrTitle", str = "Using Data Analytics to Understand Customer Needs") %>%
  ph_with_text(type = "subTitle", str = "An Introduction to Data Analytics for Business Insights")

# Add a content slide on key concepts
ppt <- ppt %>%
  add_slide(layout = "Title and Content", master = "Office Theme") %>%
  ph_with_text(type = "title", str = "Key Concepts of Data Analytics") %>%
  ph_with_text(type = "body", str = "1. Understanding customer behavior\n2. Predicting trends\n3. Personalizing services")

# Add a content slide on tools used
ppt <- ppt %>%
  add_slide(layout = "Title and Content", master = "Office Theme") %>%
  ph_with_text(type = "title", str = "Tools for Data Analytics") %>%
  ph_with_text(type = "body", str = "Popular tools include:\n- Google Analytics\n- SQL\n- R and Python\n- Tableau")

# Add a content slide on application in business
ppt <- ppt %>%
  add_slide(layout = "Title and Content", master = "Office Theme") %>%
  ph_with_text(type = "title", str = "Applying Data Insights to Business") %>%
  ph_with_text(type = "body", str = "1. Improve customer satisfaction\n2. Increase sales through targeted offers\n3. Enhance product development")

# Save the presentation
print(ppt, target = "Data_Analytics_Presentation.pptx")
getwd()

# Load necessary library
library(officer)

# Create a new PowerPoint presentation
presentation <- read_pptx()

# Add a title slide
presentation <- add_slide(presentation, layout = "Title Slide", master = "Office Theme")
presentation <- ph_with(presentation, "Using Data Analytics to Understand Customer Needs", location = ph_location_type(type = "ctrTitle"))
presentation <- ph_with(presentation, "An Introduction to Key Concepts and Applications", location = ph_location_type(type = "subTitle"))

# Add a slide about Data Analytics Concepts
presentation <- add_slide(presentation, layout = "Title and Content", master = "Office Theme")
presentation <- ph_with(presentation, "Data Analytics Concepts", location = ph_location_type(type = "title"))
presentation <- ph_with(presentation, "• What is Data Analytics?\n• Importance of Data in Business\n• Types of Data Analytics (Descriptive, Predictive, Prescriptive)", location = ph_location_type(type = "body"))

# Add a slide about Key Metrics
presentation <- add_slide(presentation, layout = "Title and Content", master = "Office Theme")
presentation <- ph_with(presentation, "Key Metrics to Understand Customers", location = ph_location_type(type = "title"))
presentation <- ph_with(presentation, "• Customer Acquisition Cost (CAC)\n• Customer Lifetime Value (CLV)\n• Churn Rate\n• Net Promoter Score (NPS)", location = ph_location_type(type = "body"))

# Add a slide about Data Sources
presentation <- add_slide(presentation, layout = "Title and Content", master = "Office Theme")
presentation <- ph_with(presentation, "Data Sources", location = ph_location_type(type = "title"))
presentation <- ph_with(presentation, "• Customer Surveys\n• Website Analytics\n• Transactional Data\n• Social Media Insights", location = ph_location_type(type = "body"))

# Add a slide about Tools
presentation <- add_slide(presentation, layout = "Title and Content", master = "Office Theme")
presentation <- ph_with(presentation, "Tools for Data Analytics", location = ph_location_type(type = "title"))
presentation <- ph_with(presentation, "• Google Analytics\n• Tableau\n• Power BI\n• R and Python", location = ph_location_type(type = "body"))

# Add a slide about EE Application
presentation <- add_slide(presentation, layout = "Title and Content", master = "Office Theme")
presentation <- ph_with(presentation, "How EE Can Benefit from Data Analytics", location = ph_location_type(type = "title"))
presentation <- ph_with(presentation, "• Enhancing Customer Experience\n• Targeted Marketing\n• Predictive Maintenance\n• Data-Driven Decision Making", location = ph_location_type(type = "body"))

# Save the presentation
print(presentation, target = "Data_Analytics_Presentation.pptx")
print(presentation, target = "Data_Analytics_Presentation.pptx")
getwd("Data_Analytics_Presentation.pptx")
