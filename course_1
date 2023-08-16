from googlesearch import search
from itertools import chain, islice

def search_courses_on_class_central(query, num_results=2):
    # Simulate searching on Class Central
    results = search(query, num=num_results, lang='en')
    return results

def search_courses_on_udemy_and_youtube(query, num_results=2):
    # Simulate searching on Udemy and YouTube
    results = search(query, num=num_results, lang='en')
    return results

if __name__ == "__main__":
    query = "best cybersecurity courses"
    num_results = 2
    
    # Search for courses on Class Central
    class_central_results = search_courses_on_class_central(query, num_results)
    
    # Search for courses on Udemy and YouTube
    udemy_and_youtube_results = search_courses_on_udemy_and_youtube(query, num_results)
    
    # Combine and limit the results to at most 5 links using itertools.islice
    all_results = chain(class_central_results, udemy_and_youtube_results)
    limited_results = islice(all_results, 5)
    
    print("Top Cybersecurity Courses:")
    for idx, link in enumerate(limited_results, start=1):
        print(f"{idx}. {link}")
