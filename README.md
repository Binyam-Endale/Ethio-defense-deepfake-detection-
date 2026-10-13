ባለብዙ-ሞዳል ዲፕፌክ ማወቂያ ስርዓት ከዋዙህ (Wazuh SIEM) ውህደት ጋር

ይህ ፕሮጀክት የተፈጠሩ የውሸት (ዲፕፌክ) ምስሎችን፣ ቪዲዮዎችን እና ድምጾችን በቅጽበት ለመለየት የሚያስችል፣ በአማርኛ እና በእንግሊዝኛ ቋንቋዎች መስራት የሚችል (Bilingual)፣ ለደህንነት ኦፕሬሽን ማዕከላት እና ድርጅቶች የተዘጋጀ የድር መተግበሪያ (Web-app) እና የሀገር ውስጥ ኦፍላይን ማወቂያ ስርዓት ነው።

አጠቃላይ መግለጫ

አርቲፊሻል ኢንተለጀንስ (AI) በፍጥነት እያደገ ሲሄድ፣ የተጭበረበሩ ሚዲያዎች እና ዲፕፌኮች የተሳሳቱ መረጃዎችን ለማሰራጨት፣ የማህበራዊ ምህንድስና ጥቃቶችን (Social Engineering Attacks) ለመፈጸም እና የድርጅቶችን ስም ለማጥፋት እየዋሉ ይገኛሉ።

ይህ ፕሮጀክት እነዚህን አደጋዎች ለመከላከል የሚያስችል ጠንካራ የረብሻ ማወቂያ መፍትሄ የሚያቀርብ ሲሆን፣ ሙሉ በሙሉ ኦፍላይን ወይም በድር/ሞባይል ሊሰራ የሚችል፣ አውቶማቲክ የ JSON ሎጎችን ከማመንጨት ባለፈ ከ Wazuh SIEM ጋር በቀጥታ በመዋሃድ የደህንነት ክትትልን የሚያደርግ ስርዓት ነው።
ዋና ዋና ባህሪያት (Key Features)ባለብዙ-ሞዳል ማወቂያ ሞተሮች (Multi-Modal Detection Engines):
የቪዲዮ ማወቂያ (Video Detection): በ 3D-CNNs ላይ የተመሰረተ ሲሆን፣ በቪዲዮው ቆይታ ውስጥ 16 የዘፈቀደ ፍሬሞችን በመውሰድ (Temporal Segment Sampling) የፊት እንቅስቃሴ መዛባቶችን እና የዲፕፌክ ምልክቶችን ይለያል።   
የድምጽ ማወቂያ (Audio Detection): የድምጽ ሞገዶችን እና ሊኒየር ፍሪኩዌንሲ ሴፕስትራል ኮፊሸንቶችን (LFCCs) በመተንተን የ AI ድምጽ ቅጂዎችን (Voice Clones) የሚለይ የሃይብሪድ CNN / Audio Fusion ኔትወርክ ይጠቀማል።   
የምስል ማወቂያ (Image Detection): በ AI የተፈጠሩ የቆዳ ሸካራማዎችን እና የጀርባ ጉድለቶችን በፒክሰል ደረጃ ለመለየት የሚረዳ 2D ResNet-18 CNN ይጠቀማል።  
ሁለገብ የቋንቋ ድጋፍ (Bilingual UI): ለአካባቢያዊ እና ክልላዊ አጠቃቀም እንዲመች ሙሉ አማርኛ እና እንግሊዝኛ ቋንቋዎችን ይደግፋል።   
SIEM / SOC ውህደት: የተዋቀሩ የ JSON ሎጎችን በቀጥታ በዋዙህ ኤጀንት (Wazuh Agent) አማካኝነት ወደ ዋዙህ ማናጀር በመላክ ቅጽበታዊ ማንቂያዎችን (Alerts) እና የደህንነት ክትትሎችን ይሰጣል።  
የሊንክ ዩአርኤል መተንተኛ (URL & Link Analyzer): የሚዲያ አገናኞችን በቀጥታ ከዩአርኤል በመቃኘት ለመፈተሽ የሚያስችል አብሮ የተሰራ መሣሪያ አለው።  
የአስተዳዳሪ መቆጣጠሪያ ፓናል (Admin Panel): ሞዴሎችን እንደገና ለማሰልጠን (Retraining)፣ የውሂብ ማህደሮችን (Datasets) ለማስተዳደር፣ የስርዓት ጤናን ለመከታተል እና ሎጎችን ለማየት የሚረዱ መሳሪያዎች አሉት።  
Flexible Deployment: በ Docker ሙሉ በሙሉ የታሸገ (Containerized) ሲሆን፣ በሊኑክስ ሰርቨሮች ላይ በአካባቢያዊ አውታረ መረቦች ወይም በልዩ ዶሜይን ስም ኦንላይን ሊሰማራ ይችላል። 

ስርዓት አርክቴክቸር (System Architecture)

አርክቴክቸሩ ለደህንነት እና ለሀብት አጠቃቀም የተመቻቹ ዋና ዋና ክፍሎችን ይዟል:
የፊት ገጽ/የድር መተግበሪያ በይነገጽ (Web Application Interface): በፒሲ እና በሞባይል መሳሪያዎች ሊደረስበት የሚችል ሁለገብ ዩአይ።  
የጀርባ ማቀነባበሪያ አገልግሎቶች (Backend Processing Services): የምስል፣ የቪዲዮ እና የድምጽ ማወቂያ ሞተሮችን የሚያስተዳድሩ የ REST API አገልግሎቶች።   
የውሂብ ጎታ እና ማከማቻ (Database & Storage Layer): ጊዜያዊ የሚዲያ ሰቀላዎችን እና ቋሚ የሜታዳታ መዝገቦችን (ሰዓት፣ የውጤት መተማመን መቶኛ፣ የማወቂያ ውጤቶች እና የኦዲት ሎጎች) የሚይዝ የሀገር ውስጥ ዳታቤዝ።   
የሎግ እና SIEM መስመር (Logging & SIEM Pipeline): ከዋዙህ SIEM ጋር በቀጥታ የተዋሃደ በ JSON የተቀረጸ የሎግ ማመንጫ ሞተር።

የውሂብ ማህደሮች እና ሞዴል ስልጠና (Datasets & Model Training)

ከፍተኛ ትክክለኛነትን ለማረጋገጥ ሞዴሎቹ በሚከተሉት መሠረታዊ መረጃዎች ተሰልጥነዋል:  
ቪዲዮ: ከታወቁ ከፍተኛ ጥራት ያላቸው መረጃዎች (HIDF, Celeb-DF v2) በተጨማሪ በ 2025 ካግል ትናንሽ የዲፕፌክ ቪዲዮ ማህደሮች ተስተካክለዋል።  
ድምጽ: ከ ASVspoof 2019 መስፈርት እና ከ SpeechFake Dataset (2024) ጋር ተቀናጅቷል።   
ምስል: Real/Fake Faces (2021) እና DeepFake-Eval-2024 የተጠቃሙ ሲሆን፣  Overfitting ለመከላከል የተለያዩ የጥንቃቄ ስልቶች ተተግብረዋል። 

Installation & Deployment
Getting Started
1.ማህደሩን ጊትሀብ ያውርዱ:

git clone https://github.com/Binyam-Endale/Ethio-defense-deepfake-detection.git

cd military-deepfake-detection

2.የፓይተን ቨርቹዋል ከባቢን በማግበር የዶከር ኮንቴይነሮቹን ያስጀምሩ

source .venv/bin/activate
sudo docker compose up -d

3.የኮንቴይነሮቹን ሁኔታ ያረጋግጡ:

sudo docker ps

4.መተግበሪያውን በ http://localhost ወይም https://www.endfcyberdefense.dpdns.org/ ማግኘት ይችላሉ።

