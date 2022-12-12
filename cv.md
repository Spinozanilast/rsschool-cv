![Текст с описанием картинки](https://i.ibb.co/CKDy62v/132005602-204671924541586-8601427056853309991-n.jpg)
# Budchanin Vadim
-----------------------------------------------
* Mails:
  * Gmail:                         vadik.trolla@gmail.com
  * Inbox:                       vadim.budchanin@inbox.ru
  * List:                              vbudchanin@list.ru
* Social:
  * [VK](https://github.com/githubuser/superlongprojectname)  
  * [Youtube](https://www.youtube.com/channel/UCqtqaziWPHAkK5xwEktgcaA)
  * [Instagram](https://www.instagram.com/spinozanilast/?hl=ru)
-----------------------------------------------
## Briefly about myself
Since **2021** I have been studying at the BNTU on the specialty ISAT (Information Systems and Technologies) at the Faculty of [FITR](https://bntu.by/faculties/fitr). And as the first Turing Award winner *Alan Jay Perlis* put it:
  > A programming language is low level when its programs require attention to the irrelevant.

Also, I suppose my occupation is a craft, with taste in the unimportant, solving problems that appear in the way of **programmers / users**.

There is no work experience (*It is supposed to be a C#-junior in the future*, do not look at my participation in this course). 
##### Strengths:
   1. Reflection
   2. Entertaining
   3. Read Richter
   4. Desire to rush into knowledge
   5. Search for deeper meaning

# Skills
I have 1.5 years of experience in programming, well, for the academic semester (except for C ++ - the year of coding) in Python and C #.
There is little experience with distributed CVS **GIT**.
Projects were developed in the following environments:
  * *Microsoft Visual Studio*, 
  * *Microsoft Visual Studio Code*, 
  * *Jetbrains IDE-s (Pycharm, Rider)*.

# Code example (project ImageViewer)
## C# (WinForms)
    private void CreatePalette()
        {
            thumbSize = 100;
            ColorsNumTextBox.Maximum = thumbSize;

            Dictionary<Color, int> colors = new Dictionary<Color, int>();

            Bitmap thumbBmp =
                new Bitmap(thumbPictureBox.Image.GetThumbnailImage(
                    thumbSize, thumbSize, ThumbnailCallback, IntPtr.Zero));

            for (int i = 0; i < thumbSize; i++)
            {
                for (int j = 0; j < thumbSize; j++)
                {
                    Color col = thumbBmp.GetPixel(i, j);
                    if (colors.ContainsKey(col))
                        colors[col]++;
                    else
                        colors.Add(col, 1);
                }
            }

            List<KeyValuePair<Color, int>> keyValueList =
                new List<KeyValuePair<Color, int>>(colors);

            keyValueList.Sort(
                delegate (KeyValuePair<Color, int> firstPair,
                KeyValuePair<Color, int> nextPair)
                {
                    return nextPair.Value.CompareTo(firstPair.Value);
                });

            AddControlstoPanel();
            for (int i = 0; i < ColorsNumTextBox.Value; i++)
            {
                palettePanel.Controls[i].BackColor = keyValueList[i].Key;
            }

            for (int j = 0; j< ColorsNumTextBox.Value; j++)
            {
                ColorDataView.Rows.Add();
                ColorDataView.Rows[j].Cells[0].Value = j;
                ColorDataView.Rows[j].Cells[1].Style.BackColor = keyValueList[j].Key;
                ColorDataView.Rows[j].Cells[2].Value = keyValueList[j].Key.R;
                ColorDataView.Rows[j].Cells[3].Value = keyValueList[j].Key.G;
                ColorDataView.Rows[j].Cells[4].Value = keyValueList[j].Key.B;
                ColorDataView.Rows[j].Cells[5].Value = keyValueList[j].Value;
            }
        } 
                                                                    
# As already mentioned, I have no work experience

# Completed trainings / courses:
  * [Version Control with Git from Epam.learn](https://learn.epam.com/detailsPage?id=601f195a-d408-4439-a16d-0630ed2a412e)
  * [Computer Science Basics](https://learn.epam.com/detailsPage?id=07464fe7-306f-4aa2-abdb-fb81ba509124)
  * PowerBi
    * [Model optimization for better performance in Power BI](https://learn.microsoft.com/ru-ru/training/modules/optimize-model-power-bi/)
    * [Introduction to creating measures with DAX in Power BI](https://learn.microsoft.com/ru-ru/training/modules/create-measures-dax-power-bi/)
    * [Designing a data model in Power BI](https://learn.microsoft.com/ru-ru/training/modules/design-model-power-bi/)

# English level - Elementary (result of Epam test is A2)
