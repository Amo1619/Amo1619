from pptx import Presentation
from pptx.util import Inches

# Create a presentation object
prs = Presentation()

# Title Slide
slide_layout = prs.slide_layouts[0]
slide = prs.slides.add_slide(slide_layout)
title = slide.shapes.title
subtitle = slide.placeholders[1]

title.text = "Analyse der Produktpolitik und Handlungsmöglichkeiten für die Traumshirt GmbH"
subtitle.text = "Eine theoretische und praktische Betrachtung\nAutoren: Ilia Fatemi, Yakub Ünnü"

# Slide 2: Einleitung
slide_layout = prs.slide_layouts[1]
slide = prs.slides.add_slide(slide_layout)
title, content = slide.shapes.title, slide.placeholders[1]

title.text = "Einleitung"
content.text = ("- Bedeutung der Produktpolitik im Marketingmix\n"
                "- Ziel der Arbeit: Analyse der Produktpolitik im theoretischen und praktischen Teil\n"
                "- Fokus: Umsatz- und Gewinnsteigerung der Traumshirt GmbH")

# Slide 3: Theorie der Produktpolitik
slide = prs.slides.add_slide(slide_layout)
title, content = slide.shapes.title, slide.placeholders[1]

title.text = "Produktpolitik: Definition und Ziele"
content.text = ("- Definition der Produktpolitik (Spiller, 2019)\n"
                "- Ziele der Produktpolitik (Haedrich/Tomczak, 1996)\n"
                "- Wichtige Aspekte: Qualität, Verpackung, Kundenservice")

# Slide 4: Aufgaben der Produktpolitik
slide = prs.slides.add_slide(slide_layout)
title, content = slide.shapes.title, slide.placeholders[1]

title.text = "Aufgaben der Produktpolitik"
content.text = ("- Einführung neuer Produkte\n"
                "- Pflege bestehender Produkte\n"
                "- Eliminierung von Produkten")

# Slide 5: Produktvariation
slide = prs.slides.add_slide(slide_layout)
title, content = slide.shapes.title, slide.placeholders[1]

title.text = "Produktvariation"
content.text = ("- Bedeutung und Vorteile (Kotler & Keller, 2016)\n"
                "- Erfolgsbeispiele: Apple, Nike, BMW")

# Slide 6: Handlungsmöglichkeiten: Influencer Marketing
slide = prs.slides.add_slide(slide_layout)
title, content = slide.shapes.title, slide.placeholders[1]

title.text = "Handlungsmöglichkeiten: Influencer Marketing"
content.text = ("- Identifizierung relevanter Influencer\n"
                "- Zusammenarbeit und Content-Erstellung\n"
                "- Cross-Promotion und Giveaways\n"
                "- Analyse und Optimierung der Kampagnen")

# Slide 7: Begründung der Handlungsmöglichkeit
slide = prs.slides.add_slide(slide_layout)
title, content = slide.shapes.title, slide.placeholders[1]

title.text = "Begründung der Handlungsmöglichkeit"
content.text = ("- Vorteile der Zusammenarbeit mit Influencern\n"
                "- Steigerung der Markenbekanntheit und des Engagements\n"
                "- Messbarkeit und Optimierung der Kampagnen")

# Slide 8: Produktdifferenzierung
slide = prs.slides.add_slide(slide_layout)
title, content = slide.shapes.title, slide.placeholders[1]

title.text = "Produktdifferenzierung"
content.text = ("- Definition und Bedeutung (Wöhe et al., 2020)\n"
                "- Methoden der Differenzierung: Design, Qualität, Funktion\n"
                "- Vorteile: Kundenbindung, Marktsegmentierung")

# Slide 9: Handlungsmöglichkeiten: Produktdifferenzierung
slide = prs.slides.add_slide(slide_layout)
title, content = slide.shapes.title, slide.placeholders[1]

title.text = "Handlungsmöglichkeiten: Produktdifferenzierung"
content.text = ("- Digitale Bewertungsbögen\n"
                "- Verbesserter Versand\n"
                "- Marktanalyse und Konkurrenzüberwachung")

# Slide 10: Produktdiversifikation
slide = prs.slides.add_slide(slide_layout)
title, content = slide.shapes.title, slide.placeholders[1]

title.text = "Produktdiversifikation"
content.text = ("- Definition und Typen: horizontal, vertikal, lateral (Spiller, 2019)\n"
                "- Vorteile: Risikominimierung, Marktentwicklung")

# Slide 11: Handlungsmöglichkeiten: Produktdiversifikation
slide = prs.slides.add_slide(slide_layout)
title, content = slide.shapes.title, slide.placeholders[1]

title.text = "Handlungsmöglichkeiten: Produktdiversifikation"
content.text = ("- Integration in die Rohstoffbeschaffung\n"
                "- Anpassungsmöglichkeiten für Kunden\n"
                "- Erweiterung in verwandte Produktkategorien\n"
                "- T-Shirt-Veredelungsdienste für Unternehmen\n"
                "- Verkauf von Fußballsachen")

# Slide 12: Zusammenfassung und Fazit
slide = prs.slides.add_slide(slide_layout)
title, content = slide.shapes.title, slide.placeholders[1]

title.text = "Zusammenfassung und Fazit"
content.text = ("- Wichtige Erkenntnisse der Produktpolitik\n"
                "- Handlungsmöglichkeiten zur Umsatz- und Gewinnsteigerung\n"
                "- Bedeutung für die Zukunft der Traumshirt GmbH")

# Slide 13: Fragen und Diskussion
slide = prs.slides.add_slide(slide_layout)
title, content = slide.shapes.title, slide.placeholders[1]

title.text = "Fragen und Diskussion"
content.text = ("- Einladung zur Diskussion\n"
                "- Beantwortung von Fragen der Zuhörer")

# Save the presentation
pptx_path = "/mnt/data/Produktpolitik_Traumshirt_GmbH.pptx"
prs.save(pptx_path)

pptx_path
