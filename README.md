
import os
import sys
import pandas as pd

from sklearn.model_selection import train_test_split
from dataclasses import dataclass

# Ingestion

@dataclass
class DataIngestionconfig:
  train_data_path: str = os.path.join('artifacts' , "train. csv")
  test_data_path: str = os.path.join('artifacts' , "test. csv")
  raw_data_path: str = os.path.join('artifacts' , "data. csv")

class DataIngestion:
  def __init__ (self) :
  self. ingestion_config=DataIngestionConfig( )
  def initiate_data_ingestion(self):
    try:
      df=pd.read_json("data.json")
    except:
      df = pd.read_csv("data.csv")

# I don't know whether the ingestion is even correct or is it right way to write.

# For data preprocessing I need to do data analysis first and get insights about how the data is ordered and I need to prepare it to a certain format.

# For error handling and i don't know what to do 

# So I don't know any thing about data engineering, I wanted to do machine learning realted task anyways I know I am not get any score here so see you again.
