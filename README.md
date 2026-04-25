# AI Real Estate Renovation Screener from Listing Photos
### What this project does

Real estate listing portals often treat photos as “visual support”, but they contain valuable information about a property’s condition. This project builds an AI based pipeline that extracts renovation signals directly from listing images and turns them into an actionable assessment of whether a property likely needs refurbishment.

The system is designed for buyer and investor use cases where the first question is not “is the property pretty”, but “what condition is it in, and what work might be required”.

### Approach

The pipeline follows a simple idea: condition depends on what room we are looking at and what finishes we can observe.

Room classification
Each image is first classified by room type, such as kitchen, bathroom, bedroom, living room.
Finish and amenity detection
For each room, the model identifies visible finishes or features that are strongly associated with renovation needs.
Examples include outdated or worn surfaces, missing amenities, or low quality finishes.
Renovation assessment
The output is an assessment of whether the detected finishes and amenities suggest that a renovation is needed, producing a renovation oriented signal that can be used in screening or prioritization.

### Results

The experiments show that the model can identify renovation relevant cues with good accuracy, providing a practical way to screen properties at scale using information that is typically ignored by standard listing filters.

### Data

All datasets used in this project, including annotated and unannotated images, are available here:
https://www.dropbox.com/scl/fo/ff6yw42k0163q1lue4ell/AFQbuJmzH-9OTrwqGmA44OE?rlkey=dl60nm207f3ngj7zwpp3i432w&st=pf039zuf&dl=0

### Final report

The full report is available here:
(https://github.com/anyols/Real-Estate-Investment-AI/releases/latest)

Reproducibility notes

This project was developed in Google Colab. If you run it in another environment, you may need to adjust file paths, dependencies, and setup steps accordingly.

### Disclaimer

Some code comments may be written in Catalan.
