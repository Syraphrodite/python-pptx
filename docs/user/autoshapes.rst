from pptx import Presentation

# Create a PowerPoint presentation object
prs = Presentation()

# Slide 1: Title Slide
slide_1 = prs.slides.add_slide(prs.slide_layouts[0])
title_1 = slide_1.shapes.title
subtitle_1 = slide_1.placeholders[1]

title_1.text = "Pastores de Bool"
subtitle_1.text = "Dance Literature, Terms, Costume, and Music"

# Slide 2: Dance Literature of the Dance
slide_2 = prs.slides.add_slide(prs.slide_layouts[1])
title_2 = slide_2.shapes.title
title_2.text = "Dance Literature of the Dance"

content_2 = slide_2.shapes.placeholders[1].text_frame
content_2.text = (
    "The 'Pastores de Bool' is a traditional folk dance from the Philippines, performed "
    "as part of Christmas celebrations. This dance reenacts the story of the shepherds' "
    "adoration of the infant Jesus. It is specifically popular in Bool, Tagbilaran City, "
    "Bohol, where it forms a part of local religious traditions. The dancers, typically "
    "composed of young girls, perform the dance while singing songs of praise and offering."
)

# Slide 3: Dance Terms Used in the Dance
slide_3 = prs.slides.add_slide(prs.slide_layouts[1])
title_3 = slide_3.shapes.title
title_3.text = "Dance Terms Used in the Dance"

content_3 = slide_3.shapes.placeholders[1].text_frame
content_3.text = (
    "1. **Saludo** – A common step in many Filipino folk dances where the dancers bow to each other.\n"
    "2. **Panadyak** – A step involving stomping or tapping the feet to the rhythm.\n"
    "3. **Pasulong** – A forward step or movement used to advance in the dance formation.\n"
    "4. **Pagtadyak** – A strong step performed with emphasis, often marking rhythm changes.\n"
    "5. **Likod-Likod** – A term describing a back-to-back position of the dancers during the performance."
)

# Slide 4: Costume
slide_4 = prs.slides.add_slide(prs.slide_layouts[1])
title_4 = slide_4.shapes.title
title_4.text = "Costume"

content_4 = slide_4.shapes.placeholders[1].text_frame
content_4.text = (
    "The costumes for Pastores de Bool are inspired by the traditional attire of shepherds in biblical times.\n\n"
    "- **Women** wear long dresses, often in bright colors, accompanied by headscarves and aprons. "
    "The dresses are modest and reflect the humble nature of the shepherds.\n\n"
    "- **Men** wear simple shirts and pants, typically in earthy tones. Some dancers carry symbolic "
    "props such as shepherd's staffs or small gifts representing offerings for the Christ Child."
)

# Slide 5: Music
slide_5 = prs.slides.add_slide(prs.slide_layouts[1])
title_5 = slide_5.shapes.title
title_5.text = "Music"

content_5 = slide_5.shapes.placeholders[1].text_frame
content_5.text = (
    "The music for Pastores de Bool is traditionally a combination of vocal singing and instrumental accompaniment.\n\n"
    "- **Vocals**: The lyrics are religious in nature, with verses praising the birth of Christ. "
    "The songs are often sung in the local dialect, enhancing the cultural significance of the dance.\n\n"
    "- **Instruments**: Simple instruments like tambourines, drums, and guitars are commonly used. "
    "The tempo of the music is typically lively, encouraging rhythmic footwork and expressive movements."
)

# Save the presentation
pptx_file = "/mnt/data/Pastores_de_Bool_Presentation.pptx"
prs.save(pptx_file)

pptx_file
