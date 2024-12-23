# Online-Quiz-system
CURRENT FEATURES
Question order randomisation,
Storing of quiz results under each user,
Previous quiz scores can be viewed on category page,
Correct answers can be shown after each question or all at once at the end,
Logged in users can return to an incomplete quiz to finish it and non-logged in users can complete a quiz if their session persists,
The quiz can be limited to one attempt per user,
Questions can be given a category,
Success rate for each category can be monitored on a progress page,
Explanation for each question result can be given,
Pass marks can be set,
Multiple choice question type,
True/False question type,
Essay question type,
Custom message displayed for those that pass or fail a quiz,
Custom permission (view_sittings) added, allowing users with that permission to view quiz results from users,
A marking page which lists completed quizzes, can be filtered by quiz or user, and is used to mark essay questions.


Requirements
django-model-utils

Installation
git clone (https://github.com/anastacia254/Online-Quiz-system.git)

pip install -r requirements.txt

Add 'quiz', 'multichoice', 'true_false', and 'essay' to your 'INSTALLED_APPS' setting.

INSTALLED_APPS = (
... 'quiz', 'multichoice', 'true_false', ...
)

Add the following to your projects 'urls.py' file, substituting 'q' for whatever you want the quiz base url to be.

urlpatterns = patterns('',
... url(r'^q/', include('quiz.urls')), ...
)
