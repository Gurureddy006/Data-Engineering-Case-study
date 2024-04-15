
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

