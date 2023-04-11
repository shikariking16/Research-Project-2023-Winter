# Code Overview
There are two functions in this code that are used to scrape either Reddit or Stackoverflow.

## Reddit Scraper

reddit_subreddit_scraper(sub_reddit, db_name, client_id, client_secret, user_agent,uri,start_date, end_date)

    This function seaches a subReddit on reddit and adds the information to a MongoDB database.
    
    Parameters:
        sub_reddit(String) = Sub reddit name
        db_name(String) = What you want the database called
        client_id(String) = The client ID given from Reddit API
        client_secret(String) = Secret given by Reddit API
        user_agent(String) = Username of the user
        uri(String) = The link to the MongoDB database 
        start_date(datetime)= The earliest posts created that can be collected
        end_date(datetime) = The latest a post can be collected

## Stackoverflow Scraper

stackoverflow_scraper(tag, keyword, db_name, user_agent, uri, fromDate, toDate)

    This function searches for Stack Overflow questions with a certain tag and saves the information to a MongoDB database.
    As well as saving the user information.
    
    Parameters:
        tag(String) = Tag name
        keyword(String) = Keyword to search in titles and body of questions
        db_name(String) = What you want the database called
        user_agent(String) = User agent name
        uri(String) = The link to the MongoDB database 
        fraomDate(Datetime) = What date to start scrapping 
        toDate(Datetime) = The end date to end scrapping
