# Dictionary1
First iteration in trying to create a khasi-khasi dictionary

# Python File structure and purpose
    1_test_internetarchive_api.ipynb - downloads khasi pdfs 
    2_dictionary_code.ipynb - main file
    3_freedict.ipynb - attempt using freedict
    4_llama.ipynb - attempt using llama
    5_clean_corpus.ipynb - read the corpus and clean. Extract vocabulary. Extract sentences.
    6_scraping_for_corpus.ipynb - attempt to scrape a large Khasi corpus from the internet

# Folder contents
    downloads - pdf files that can be read selected from download2
    downloads2 - pdf files downloaded from internetarchive

# Activities Log
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
        