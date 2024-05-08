use role accountadmin;      -- select role
use warehouse compute_wh;   -- select compute

-- cretae database called cricket and 4 schemas
CREATE DATABASE IF NOT EXISTS CRICKET;
CREATE OR REPLACE SCHEMA CRICKET.LAND;
CREATE OR REPLACE SCHEMA CRICKET.RAW;
CREATE OR REPLACE SCHEMA CRICKET.CLEAN;
CREATE OR REPLACE SCHEMA CRICKET.CONSUMPTION;

--Check the Schema
show schemas in DATABASE CRICKET;

--change context
USE SCHEMA CRICKET.LAND;

--create json file format
CREATE OR REPLACE FILE FORMAT CRICKET.LAND.MY_JSON_FORMAT
    type = json
    null_if = ('\\n', 'null', '')
    strip_outer_array = true
    comment = 'json File Format with outer strip array flag true'

--create an internal stage
CREATE OR REPLACE STAGE CRICKET.LAND.MY_STG 

--check file in just created stage
LIST @CRICKET.LAND.MY_STG
