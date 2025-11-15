
from reportlab.lib.pagesizes import letter
from reportlab.platypus import SimpleDocTemplate, Paragraph
from reportlab.lib.styles import getSampleStyleSheet
doc = SimpleDocTemplate("output.pdf", pagesize=letter)
styles = getSampleStyleSheet()
content = [
Paragraph("Single Page PDF Example", styles["Title"]),
Paragraph("This PDF contains example code on a single page.", styles["Normal"]),
]
doc.build(content)
