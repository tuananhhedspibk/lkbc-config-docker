FROM biencosi/deepdive

WORKDIR home

COPY ddlib/gen_feats.py ./ddlib
COPY ddlib/handle_string.py ./ddlib

RUN rm /root/local/lib/python/ddlib/gen_feats.py && \
  mv ddlib/gen_feats.py /root/local/lib/python/ddlib/ && \
  mv ddlib/handle_string.py /root/local/lib/python/ddlib/

RUN mkdir vnlaw-deepdive && \
  cd vnlaw-deepdive

COPY vnlaw-deepdive_2/ ./vnlaw-deepdive

RUN curl -O https://bootstrap.pypa.io/get-pip.py && \
  python get-pip.py

RUN pip install numpy && \
  pip install scipy && \
  pip install pathlib && \
  pip install pyvi

RUN export DEEPDIVE_UNLOAD_MATERIALIZED=false
