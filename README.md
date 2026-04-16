import streamlit as st
import pyqrcode
import  png

mail=st.text_input("Gmail Adresiniz")
telefon="905415353305"
# top sizde
link="https://wa.me/"+telefon+"?text="+mail

qr = pyqrcode.create(link)
qr.png("wp.png",scale=13)

st.image("wp.png")
