# 유해물질 법인별 양산보증 측정 현황!

b = (
    Bar()
    .add_xaxis(["Microsoft", "Amazon", "IBM", "Oracle", "Google", "Alibaba"])
    .add_yaxis("2017-2018 Revenue in (billion $)", random.sample(range(100), 10))
    .set_global_opts(
        title_opts=opts.TitleOpts(
            title="Top cloud providers 2018", subtitle="2017-2018 Revenue"
        ),
        toolbox_opts=opts.ToolboxOpts(),
    )
)
st_pyecharts(
    b, key="echarts"
)  # Add key argument to not remount component at every Streamlit run
st.button("Randomize data")
