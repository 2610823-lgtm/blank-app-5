import streamlit as st

# 앱 제목 설정
st.title("🍿 영화관 세트 메뉴 구성기")
st.subheader("가능한 모든 메뉴 조합을 확인해보세요!")

# 원본 데이터 구조 유지
popcorn_options = ["기본", "카라멜", "어니언"]
drink_options = ["생수", "탄산음료"]

st.markdown("---")

# 원본 반복문 로직 유지하며 스트림릿 화면에 출력
for popcorn in popcorn_options:
    for drink in drink_options:
        # st.write를 사용하여 웹 화면에 출력 (drink 오타 수정 포함)
        st.write(f"🎬 **세트메뉴:** {popcorn} 팝콘, {drink}")

st.markdown("---")