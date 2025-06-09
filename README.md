# Dictionary1
First iteration in trying to create a khasi-khasi dictionary

# Python File structure and purpose
    1_test_internetarchive_api.ipynb - downloads khasi pdfs 
    2_dictionary_code.ipynb - main file
    3_freedict.ipynb - attempt using freedict
    4_llama.ipynb - attempt using llama
    5_clean_corpus.ipynb - read the corpus and clean. Extract vocabulary. Extract sentences.
    5.2_extract_sentences.ipynb - extract sentences from corpus
    5.3_extract_full_sentences.ipynb - extract full sentences not delimited by new lines.
    5.4_verify_vocabulary.ipynb - extract vocabulary from cleaned sentences
    6_scraping_for_corpus.ipynb - attempt to scrape a large Khasi corpus from the internet
    7_extract_meanings.ipynb - creates embeddings for semantics

# Folder contents
    downloads - pdf files downloaded from internet archive where text can be selected
    downloads_newspapers - files scraped from newspapers
    downloads_ocr - pdf files downloaded from internet archive in ocr format
    downloads_text - pdf files downloaded from internet archive in text format
    outputs - all output files and folders
        vocabulary - vocabulary collected from files in downloads_ocr
        sentences - contains files that list lines scanned from downloads_ocr
        full_sentences - contains files that list a complete sentence on each line extracted from sentences folder 
        collected_vocabulary - vocabulary collected from files in full_sentences folder

# Activities Log
    9.6.2025
        # use tesseract and clean files to collect full sentences for semantic training
    1.5.2025
        # Text format of Khasi books do not preserve special characters such as Ñ ñ
        # Used tesseract set to spa+fra (Spanish+France) to recognise special characters
        # Create vocabulary from each book
    31.5.2025
        # Read papers on Khasi Corpus : Sunita Warjri and Medari Tham 
        # Download Khasi Pos tagger and Khasi Pos corpus
        # Create a text corpus from the downloaded text files
        # Read corpus to get the words
        # Read dictionary and POS to tag the words
    30.5.2025
        # Try mistral - was terrible for Khasi language
        # Try phi - was terrible for Khasi
        # Understood that I want to develop a model that will find the meaning of a word in Khasi language
        # Download Ollama | Download llama-cpp-python

# Errors log
    31.5.2025
        # VSCode was not changing environment and kept using the system-wide python and modules
            # Solution is to check the upper right corner where there is an option to select kernel. Then select the desired interpreter as 'khasi-env'
        